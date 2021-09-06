# Rust Box<T>

`Box <T>`是一个智慧指标，指向在型别为T的堆上分配的资料。允许将资料储存在堆而不是堆叠上。是一个拥有的指标。除了将资料储存在堆上之外，当`Box <T>`

`Box <T>`
`Box`
`Box`

使用 主要是，下面通过一个简单的例子来理解这一点：`Box <T>`
`Box <T>`

```rust
fn main()  
{  
  let a = Box :: new(1);  
  print!("value of a is : {}",a);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
value of a is : 1
```

在上面的例子中，如果存取 当程式结束时，储存在堆叠中，它指向的资料储存在堆上。`a``1``Box``Box``Box``Box`

下面来看看上面例子的图解表示：

![img](https://tw511.com/upload/images/201910/20191014013950410.png)

**Cons列表**

- `Cons`代表「构造功能」。
- `Cons`列表是一个资料结构，用于从两个引数构造一个新对，这对称为`List`
- 假设有两个元素`x` `y` `cons` `cons 「x到y」` `x` `y`
- `Cons`列表包含两个元素，即当前项和最后一项。由于`Nil` `Nil`

现在，建立包含`cons`

```rust
enum List  
{  
   cons(i32, List),  
   Nil,  
}
```

在上面的程式码中，建立了`List` `i32` `cons`

现在，在以下范例中使用上面的`List`

```rust
enum List {  
    Cons(i32, List),  
    Nil,  
}  
use List::{Cons, Nil};  
fn main()  
{  
  let list = List::Cons(1,Cons(2,Cons(3,Nil)));  
  for i in list.iter()  
  {  
    print!("{}",i);  
  }  
}
```

执行上范例程式码，得到以下结果 -

![img](https://tw511.com/upload/images/201910/20191014013951411.png)

在上面的范例中，Rust编译器丢掷错误「具有无限大小」，因为List型别包含递回的变体。因此，Rust无法找出储存List值所需的空间。使用`Box <T>`

## 使用`Box <T>`

Rust无法确定储存递回资料型别需要多少空间。Rust编译器在前一种情况下显示错误：

```shell
= help: insert indirection (e.g., a 'Box', 'Rc', or '&') at some point to make 'List' representable
```

在上面的例子中，可以使用 指标的大小在程式执行期间不会改变。指标指向将储存在堆上而不是 指标可以直接放在`Box <T>` `Box <T>` `Box <T>` `Box <T>` `cons` `Box <T>` `cons`

![img](https://tw511.com/upload/images/201910/20191014013951412.png)

下面来看一个简单的例子 -

```rust
#[derive(Debug)]   
enum List {  
    Cons(i32, Box<List>),  
    Nil,  
}  
use List::{Cons, Nil};  
fn main()  
{  
  let list = Cons(1,Box::new(Cons(2,Box::new(Cons(3,Box::new(Nil))))));  

    print!("{:?}",list);  

}
```

执行上面范例程式码，得到以输出结果如下 -
```
  Cons(1, Cons(2, Cons(3, Nil)))
```
