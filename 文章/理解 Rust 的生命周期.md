# 理解 Rust 的生命周期

作者：丹尼尔·P·克拉克

原文链接：https://www.cloudbees.com/blog/lifetimes-in-rust

高级语言很方便地处理我们代码中的每个对象的存活的范围(`scope`), 我们不需要理解这些对象的生命周期。Rust同样为我们管理着生命周期，我们可以通过所有权(`ownership`)和借用(`borrowing`)对简单情况进行更多的控制,但是对于复杂的情况，我们需要在代码中给出识别标识，以便编译器能够理解更大的生命周期的范围。

简单的说，一切的一切归根结底都是为了在对象使用完之后就释放它。高级语言如Go、Ruby、Python等等，使用垃圾回收器在整个代码中扫描和标记对象，以查看它们是否准备好从内存中释放掉，并将对所有已标记可释放的对象执行释放操作。当你不再使用对象时，低级语言如C、汇编要求你手工释放它们。

Rust避免了垃圾回收和手写代码释放内存的成本，它根据代码库中每个对象的生命周期维护释放内存的时间。生存期主要由所有权系统决定（描述代码的哪个部分负责拥有内存中对象的系统），以及在复杂情况下，由帮助编译器而提供的手动生命周期描述符来决定。一旦对象的生命周期束，内存将立即释放。

## 简单的生命周期

Rust的**const**类型的生命周期是整个程序，它的值可以内联到代码中的任何地方。

```rust
const MAJOR_VERSION: i32 = 1;
```

**static**类型的生命周期也是整个程序，但它不会被内联，它存在于内存的固定位置。

```rust
static MINOR_VERSION: i32 = 0;
```

大多数其他对象的生命周期只发生在块(`block`)的范围内，或者直到某个方法调用夺走了它们的所有权。如果一个对象要在方法调用中超出其使用范围而存在(意思是方法调用完还继续存活)，那么该方法需要借用(`borrow`)它，或者复制(`copy`)它，以便在方法完成后，它的生命周期可以在外部作用域中继续长存。

```rust
let money: String = "42".to_string();
fn borrow_it(qty: &String) {
  println!("Your money total is ${}", qty)
}
borrow_it(&money); // borrowed ownership
// the ownership of money has been returned to this higher scope
fn consume_it(qty: String) {
  println!("My money total is ${}", qty)
}
consume_it(money);
// money memory is freed as the ownership has been
// taken into the methods scope and that scope has ended.
println!("No money: ${}", money);
// This fails
```

当我们运行上面的代码的时候，Rust会告诉我们哪里出错了:

```rust
error[E0382]: use of moved value: `money`
  --> src/main.rs:19:29
   |
15 |   consume_it(money);
   |              ----- value moved here
...
19 |   println!("No money: ${}", money);
   |                             ^^^^^ value used here after move
   |
   = note: move occurs because `money` has type `std::string::String`, which does not implement the `Copy` trait
```

请注意，它告诉我们，如果`std::string::String`如果实现了`Copy trait`，我们的代码就可以工作。如果您将上述代码更改为使用`i32`类型而不是String，它将正常地工作；`i32`确实实现了`Copy trait`，编译器将从块中的用法推断出该值稍后将被使用，因此在这种情况下，将在借用时执行复制。即使复制后，money的生命周期也会在最后一次使用时结束，因为它会被最后的`println!`命令所使用。

## 复杂的生命周期

有时候，当代码中没有足够的信息来确定生命周期时，Rust编译器会要求描述/注释生命周期。

```rust
// 地球
#[derive(Debug)]
struct Earth {
  location: String,
}
// 恐龙
#[derive(Debug)]
struct Dinosaur<'a> {
  location: &'a Earth,
  name: String,
}
fn main() {
  let new_york = Earth {
    location: "New York, NY".to_string(),
  };
  let t_rex = Dinosaur {
    location: &new_york,
    name: "T Rex".to_string(),
  };
  println!("{:?}", t_rex);
}
```

在上面的例子中，你可以看到一个生命周期的注释`'a`。当我们的struct借用`Earth`实例的时候, 它需要增加生命周期标识，它会帮助编译器理解🦕恐龙(`Dinosaur`)不能比🌍地球(`Earth`)还长寿，因为它引用了Earth。

当我第一次在自己的项目中处理实现和学习生命周期的时候，有一个技巧帮助了我。当程序建议需要它们时，就是在它们可能不需要放置的地方放置了更多的生命周期引用。我发现编译器的错误消息在“生命周期注释存在并且错误时”比“不存在和错误时”更能理解我的意图。当然，我建议查看实现了生存期的代码，以帮助您开始工作。一点点的尝试和错误将帮助您快速理解。

上面恐龙的一个示例`impl`代码如下：

```rust
impl<'a> From<Dinosaur<'a>> for String {
  fn from(d: Dinosaur) -> String {
    format!("{:?}", d)
  }
}
// replace the above println! with
println!("{}", String::from(t_rex));
```

## 范围生命周期

当需要从一个底层的或者内部(lower/inner)的scope中获取值时， 最好的方法就是把需要的结果值赋值给更高的scope中的变量:

```rust
{
  // outer scope
  let result: i32;
  {
    // inner scope
    result = 42 + 42;
  }
  println!("{}", result);
}
```

如果我们尝试在内部的scope中将结果直接赋值给外部的变量而没有预先声明它，我们会得到如下的错误：

```rust
error[E0425]: cannot find value `result` in this scope
  --> src/main.rs:10:18
   |
10 |   println!("{}", result);
   |                  ^^^^^^ not found in this scope
```

这是因为在inner scope中对象的生命周期只限于inner scope, 除非它们被赋值给外部的更长的scope中的对象。返回值可以看作是外部的scope的对象。我们改造一下上面的例子：

```rust
{
  let result: i32 = {
    42 + 42
  };
  println!("{}", result);
}
```

正常输出 84。

当我们没有正确使用scope时编译器会洞悉到我们的错误。所以我们直接写我们认为正确的代码就好了，简单按照编译的反馈信息修改我们的错误就好了，这里有个错误的例子：

```rust
{
  let result: &i32;
  
  {
    let x = 42 + 42;
    result = &x;
  }
  println!("{}", result);
}
```

编译它:

```rust
error[E0597]: `x` does not live long enough
  --> src/main.rs:7:3
   |
6  |     result = &x;
   |               - borrow occurs here
7  |   }
   |   ^ `x` dropped here while still borrowed
...
10 | }
   | - borrowed value needs to live until here
```

这里输出很清晰的生命周期图。或者使用`clone`或者使用`copy`等手段可以把值返回给更高的scope。但是这经常会带来一些性能上的影响因为复制内存中的数据要比传引用要化更长的时间。

## 总结

在Rust所有涉及生命周期的事情中，注释似乎是一个很大的障碍，因为语法看起来有点过时。但重要的是，当你使用它们的时候，你不会改变它们的方式——你其实只是简单地宣布它们。也就是说，有注释的生命周期与没有写注释的生命周期的工作方式是相同的。它们只是帮助编译器澄清生命周期所涉及的上下文的标记。
除此之外，生命周期很简单。只需编写代码，看看会发生什么。Rust语言的编译器将是您的导师，您的理解将随着您从编译器非常智能的错误消息中学习而增长。你可以大胆地编码，因为Rust可以帮助你在未知的海洋中遨游。
