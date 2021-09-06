# Rust Deref trait

`Deref <T> trait`用于自定义解除参照运算子( 如果实现 因此，在参照上工作的程式码也可以用在智慧指标上。`*`
`Deref <T>`

## 常规参照

常规参照是一种指向某个值的指标，该值储存在其他地方。下面来看一个简单的例子来建立`i32` `this`

```rust
fn main()  
{  
  let a = 20;  
  let b = &a;  
  if a==*b  
  {  
    println!("a and *b are equal");  
  }  

  else  
  {  
    println!("they are not equal");  
  }  
}
```

执行上面范例程式码，得到以下结果 -

```shell
a and *b are equal
```

在上面的例子中，如果使用 因此，可以比较变数 如果使用`a` `i32` `20` `b` `a` `* b` `20` `a` `* b` `&b` `* b`

## `Box <T>`作为参照

`Box <T>`指标可用作参照。

下面来看一个简单的例子：

```rust
fn main()  
{  
  let a = 11;  
  let b = Box::new(a);  
  print!("Value of *b is {}",*b);  
}
```

输出结果如下所示 -

```shell
Value of *b is 11
```

在上面的范例中，它们之间的唯一区别是b包含指向资料的框，而不是通过使用`Box <T>` `&`

## 智慧指标作为参照

现在，建立类似于`Box <T>`

`Box <T>`可以定义为具有一个元素的元组结构，例如 建立元组结构后，在`MyBox <T>`
`MyBox <T>`

下面来看一个简单的例子：

```rust
struct MyBox<T>(T);  
impl<T> MyBox<T>  
{  
  fn example(y : T)->MyBox<T>  
  {  
    MyBox(y)  
  }  
}  
fn main()  
{  
  let a = 8;  
  let b = MyBox::example(a);  
  print!("Value of *b is {}",*b);  
}
```

执行上面范例程式码，得到以下结果 -

![img](https://tw511.com/upload/images/201910/20191014013953413.png)

在上面的例子中，建立了智慧指标 因此得出结论，无法取消类似于`b` `Box <T>`

## 实现Deref Trait

- `Deref Trait`在标准库中定义，该库用于实现名为`deref`
- `deref`方法借用`self`

下面来看一个简单的例子：

```rust
struct MyBox<T>  
{  
  a : T,  
}  
use :: std::ops::Deref;  
impl<T> Deref for MyBox<T>  
{  
  type Target = T;  
  fn deref(&self) ->&T  
  {  
    &self.a  
  }  
}  
fn main()  
{  
  let b = MyBox{a : 10};  
  print!("{}",*(b.deref()));  
}
```

执行上面范例程式码，得到以下结果 -

```shell
10
```

**程式说明**

- `Deref trait`在`MyBox`
- `Deref trait`实现`deref()` `deref()` `a`
- `type Target = T;`是 关联型别用于宣告泛型型别引数。`Deref trait`
- 建立了`MyBox` `b`
- 通过使用`MyBox``b.deref()` `deref()` `deref()`

## Deref强制

- `Deref`强制是将实现`Deref trait` `Deref`
- `Deref`强制是对函式和方法的引数执行的。
- 当将特定型别的参照传递给与函式定义中的引数型别不匹配的函式时，`Deref`

下面来看一个简单的例子：

```rust
struct MyBox<T>(T);  
use :: std::ops::Deref;  
impl<T> MyBox<T>  
{  
  fn hello(x:T)->MyBox<T>  
  {  
    MyBox(x)  
  }  
}  
impl<T> Deref for MyBox<T>  
{  
  type Target = T;  
  fn deref(&self) ->&T  
  {  
    &self.0  
  }  
}  
fn print(m : &i32)  
{  
  print!("{}",m);  
}  
fn main()  
{  
  let b = MyBox::hello(5);  

  print(&b);  
}
```

执行上面范例程式码，得到以下结果 -

```
5
```

在上面的例子中，使用引数 在这种情况下，实现`＆b` `print(&b)` `&Box <i32>` `Deref trait` `Deref` `&Box <i32>` `&i32`

## Derif强制与可变性的相互作用

到目前为止，使用`Deref Trait` `*` `DerefMut Trait` `*`

Rust在以下三种情况下执行`Deref`

- 当T：`Deref <Target = U>` `T` `U` `&T` `&U`
- 当T：`DerefMut <Target = U>` `T` `U` `&mut T` `&mut U`
- 当T：`Deref <Target = U>` `T` `U` `&mut T` `&U`
