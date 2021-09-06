# Rust生命周期

生命周期定义了参照有效的范围。生命周期是隐含的和推断的。Rust使用通用生命周期引数来确保使用有效的实际参照。

## 预防与生命周期的悬空参照

当程式试图存取无效参照时称为悬空参照，所指向无效资源的指标称为悬空指标。

看看一个简单的例子：

```rust
fn main()  
{  
  let a;  
  {  
    let b = 10;  
     a = &b;  
  }  
  println!("a : {}",a);  
}
```

输出结果如下 -

![img](https://tw511.com/upload/images/201910/20191014013947406.png)

在上面的范例中，外部作用域包含 内部范围包含变数 变数的参照储存在变数 当内部范围结束时，尝试存取 Rust编译器将丢掷一个编译错误，因为 Rust将使用借用检查器确定程式码无效。`a` `b` `10` `b` `a` `a` `a`

## 借用检查器

借用检查器用于解决悬挂参照的问题。借用检查器用于比较范围以确定它们是否有效。

![img](https://tw511.com/upload/images/201910/20191014013947407.png)

在上面的例子中，注释了 在编译时，Rust将拒绝该程式，因为 可以修复上面的程式码，以便不会发生编译器错误。`a` `a` `b` `b` `a` `b`

![img](https://tw511.com/upload/images/201910/20191014013947408.png)

在上面的例子中，因此，上面的程式码执行时没有任何编译错误。`a` `b`

## 生命周期注释语法

- 生命周期注释不会改变任何参照的生存时间。
- 函式还可以使用泛型生存期引数接受任何生命周期的参照。
- 生命周期注释描述了多个引数的生命周期之间的关系。

**生命周期注释语法应遵循的步骤：**

- 生命周期引数的名称应以(`'`
- 它们主要是小写和简写。例如：`'a`
- 生命周期引数注释放在参照的`&`

**生命周期注释语法的一些范例：**

- `&i32` // reference
- `& 'a i32` // reference with a given lifetime.
- `& 'a mut i32` // mutable reference with a given lifetime.

## 函式签名中的生命周期注释

```
'a`代表参考的生命周期。每个参考都有与之相关的生命周期。也可以在函式签名中使用生命周期注释。通用生命周期引数在角括号`<>
```

范例 -

```rust
fn fun<'a>(...);
```

在上面的例子中，如果函式包含两个具有两个不同生命周期的参考引数，则它可以表示为：`fun` `'a`

```rust
fn fun<'a,'b>(...);
```

如果`'y'`

```rust
fn fun<'a>(y : & 'a i32);
```

如果`'y'`

```rust
fn fun<'a>(y : & 'a mut i32);
```

两个 唯一的区别是`&'a i32``&'a mut i32``'a``&``mut`

`&mut i32`的意思是「对i32的可变参照」。表示「对具有生命周期'的
`&'a mut i32` `i32`

## 结构中的生命周期注释

也可以在结构中使用显式生命周期，就像在函式中使用的一样。

下面来看看一个范例：

```rust
struct Example  
   x : & 'a i32,  //  x is a variable of type i32 that has the lifetime 'a.
```

下面来看一个简单的例子：

```rust
struct Example<'a> {  
    x: &'a i32,  
}  
fn main() {  
    let y = &9;   
    let b = Example{ x: y };  
    println!("{}", b.x);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
9
```

### impl块

可以实现具有生命周期`'a` `impl`

下面来看一个简单的例子：

```rust
struct Example<'a> {  
    x: &'a i32,  
}  
impl<'a> Example<'a>  
{  
fn display(&self)  
{  
  print!("Value of x is : {}",self.x);  
}  
}  
fn main() {  
    let y = &90;   
    let b = Example{ x: y };  
    b.display();  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Value of x is : 90
```

## 多个生命周期

有两种可能性：

- 多个参照具有相同的生命周期。
- 多个参照具有不同的生命周期。

当参照具有相同的生命周期时。

```rust
fn fun <'a>(x: & 'a i32 , y: & 'a i32) -> & 'a i32  

   //block of code.
```

在上述情况下，参照`x` `y` `'a`

当参照具有不同的生命周期时。如下 -

```rust
fn fun<'a , 'b>(x: & 'a i32 , y: & 'b i32)   

   // block of code.
```

在上述情况下，参考`x` `y` `'a` `'b`

**'static**

`'static`的生命周期是特殊的生命周期。它表示某些东西具有生命周期 主要是 具有「静态生命周期」的参照对整个程式有效。`'static` `'static`

范例：

```rust
let s : & 'static str = "Yiibai tutorial" ;
```

## 生命周期椭圆

生命周期椭圆是一种推理演算法，它使常见的模式更符合人体工程学。生命周期椭圆使一个程式被淘汰。

生命周期椭圆可以在任何地方使用：

- `& 'a T`
- `& 'a mut T`
- `T<'a>`

生命周期椭圆可以以两种方式出现：

- **输入生命周期**
- **输出生存期**

范例 -
```rust
fn fun<'a>( x : & 'a i32);                       // input lifetime  
fn fun<'a>() -> & 'a i32;                      // output lifetime  
fn fun<'a>(x : & 'a i32)-> & 'a i32;      // Both input and output lifetime.
```
