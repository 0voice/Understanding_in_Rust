# Rust Trait

Rust trait 是Rust语言的一个特性(性状)，它描述了它可以提供的每种型别的功能。性状类似于其他语言中定义的介面的特征。性状是一种对方法签名进行分组以定义一组行为的方法。使用


`trait`

`trait`的语法：

```rust
trait trait_name  
//body of the trait.
```

在上面的例子中，宣告特征后跟特征(性状)名称。在大括号内，宣告方法签名以描述实现特征的型别的行为。

下面来看一个简单的例子：

```rust
struct Triangle  
{  
  base : f64,  
  height : f64,  
}  
trait HasArea  
{  
  fn area(&self)->f64;  
}  

impl HasArea for Triangle  
{  
  fn area(&self)->f64  
  {  
    0.5*(self.base*self.height)  
  }  
}  
fn main()  
{  
  let a = Triangle{base:10.5,height:17.4};  
  let triangle_area = a.area();  
  println!("Area of a triangle is {}",triangle_area);   
}
```

执行上面范例程式码，得到以下结果 -

```shell
Area of a triangle is 91.35
```

在上面的例子中，宣告了一个 是在 通过使用结构的范例，即`HasArea` `area()` `HasArea` `Triangle` `a.area()` `area()`

## 性状作为引数

特征(性状)也可以用作许多不同型别的引数。

上面的例子实现了 可以定义呼叫`HasArea` `area()` `area()` `calculate_area()` `HasArea` `area()`

下面来来看看语法：

```rust
fn calculate_area(item : impl HasArea)  
  println!("Area of the triangle is : {}",item.area());  
}
```

## 性状限制了通用函式

性状很有用，因为它们描述了不同方法的行为。但是，通用函式不遵循此约束。通过一个简单的场景来理解这一点：

```rust
fn calculate_area<T>( item : T)  
   println!(?Area of a triangle is {}?, item.area());
```

在上面的例子中，Rust编译器丢掷「没有找到型别为 如果将性状系结到泛型`T` `T`

```rust
fn calculate_area<T : HasArea> (item : T)  
{  
    println!("Area of a triangle is {} ",item.area());  
}
```

在上面的例子中，Rust编译器知道任何实现`<T:HasArea>` `T` `HasArea` `HasArea` `area()`

下面来看一个简单的例子：

```rust
trait HasArea  
{  
  fn area(&self)->f64;  
}  
struct Triangle  
{  
  base : f64,  
  height : f64,  
}  

impl HasArea for Triangle  
{  
  fn area(&self)->f64  
  {  
    0.5*(self.base*self.height)  
  }  
}  
struct Square  
{  
  side : f64,  
}  

impl HasArea for Square  
{  
  fn area(&self)->f64  
  {  
     self.side*self.side  
  }  
}  
fn calculate_area<T : HasArea>(item : T)  
{  
  println!("Area is : {}",item.area());  
}  

fn main()  
{  
  let a = Triangle{base:10.5,height:17.4};  
  let b = Square{side : 4.5};  
  calculate_area(a);  
  calculate_area(b);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Area is : 91.35
Area is : 20.25
```

在上面的例子中，`calculate_area()``T`

## 实施性状的规则

实现性状有两个限制：

- 如果范围中未定义性状，则无法在任何资料型别上实现该性状。

下面来看一个简单的例子：

```rust
use::std::fs::File;  
fn main()  
{  
  let mut f = File::create("hello.txt");  
  let str = "Yiibai";  
  let result = f.write(str);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
error : no method named 'write' found.
           let result = f.write(str);
```

在上面的例子中，Rust编译器丢掷一个错误，即 因此，需要使用`"no method named 'write' found"` `use::std::fs::File;` `write()` `Write trait`

- 正在实现的性状必须定义。例如：如果定义 但是，无法为型别`HasArea` `i32` `i32` `toString`

## 多个性状界限

使用`'+'`

如果想系结多个性状，可使用`+`

下面来看一个简单的例子：

```rust
use std::fmt::{Debug, Display};  
fn compare_prints<T: Debug + Display>(t: &T)  
{  
    println!("Debug: '{:?}'", t);  
    println!("Display: '{}'", t);  
}  

fn main() {  
    let string = "Yiibai";  
    compare_prints(&string);  
}
```

执行上面范例程式码，输出结果如下 -

```shell
Debug: ' "Yiibai"'
Display: ' Yiibai'
```

在上面的范例中，`Display` `Debug` `+` `T`

使用`where`

- 使用出现在括号`{` `where`
- `where`子句也可以应用于任意型别。
- 当使用`where`

如下程式码 -

```rust
fn fun<T: Display+Debug, V: Clone+Debug>(t:T,v:V)->i32  
//block of code;
```

在上述情况下使用`where`

```rust
fn fun<T, V>(t:T, v:V)->i32  
  where T : Display+ Debug,   
             V : Clone+ Debug  

       //block of code;
```

在上面的例子中，使用`where`

下面来看看一个简单的例子：

```rust
trait Perimeter  
{  
  fn a(&self)->f64;  
}  
struct Square  
{  
  side : f64,  
}  
impl Perimeter for Square  
{  
  fn a(&self)->f64  
  {  
    4.0*self.side  
  }  
}  
struct Rectangle  
{  
 length : f64,  
 breadth : f64,  
}  
impl Perimeter for Rectangle  

{  
 fn a(&self)->f64  
 {  
   2.0*(self.length+self.breadth)  
 }  
}  
fn print_perimeter<Square,Rectangle>(s:Square,r:Rectangle)  
  where Square : Perimeter,  
        Rectangle : Perimeter  
        {  
          let r1 = s.a();  
          let r2 = r.a();  
          println!("Perimeter of a square is {}",r1);  
          println!("Perimeter of a rectangle is {}",r2);  
        }  
fn main()  
{  
    let sq = Square{side : 6.2};  
    let rect = Rectangle{length : 3.2,breadth:5.6};  
    print_perimeter(sq,rect);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Perimeter of a square is 24.8
Perimeter of a rectangle is 17.6
```

## 预设方法

可以将预设方法新增到性状定义的方法定义为已知。范例程式码：

```rust
trait Sample  

  fn a(&self);  
  fn b(&self)  
  {  
      println!("Print b");  
  }
```

在上面的例子中，预设行为被新增到性状定义中。还可以覆盖预设行为。下面通过一个例子看看这个场景：

```rust
trait Sample  
{  
 fn a(&self);  
 fn b(&self)  
 {  
   println!("Print b");  
 }   
}   

struct Example  
{  
 a:i32,  
 b:i32,  
}  



impl Sample for Example  
{  
  fn a(&self)  
  {  
    println!("Value of a is {}",self.a);  
  }  

  fn b(&self)  
  {  
    println!("Value of b is {}",self.b);  
  }  
}  
fn main()  
{  
  let r = Example{a:5,b:7};  
  r.a();  
  r.b();    
}
```

执行上面范例程式码，得到以下结果 -

```shell
Value of a is : 5
Value of b is : 7
```

在上面的例子中，因此得出结论，可覆盖性状中定义的方法。`b()`

## 继承

从另一个性状派生的性状称为继承。有时，有必要实现另一个性状的性状。如果想从'A'性状继承'B'性状，那么它看起来像：

```rust
trait B : A;
```

参考以下一段完整的程式码 -

```rust
trait A  
{  
  fn f(&self);  
}  
trait B : A  
{  
  fn t(&self);  
}  
struct Example  
{  
  first : String,  
  second : String,  
}  
impl A for Example  
{  
  fn f(&self)  
  {  

   print!("{} ",self.first);  
  }  

 }  
 impl B for Example  
 {  
  fn t(&self)  
  {  
    print!("{}",self.second);  
  }  
}  
fn main()  
{  
  let s = Example{first:String::from("Yiibai"),second:String::from("tutorial")};  
  s.f();  
  s.t();  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Yiibai tutorial
```

在上面的例子中，程式实现'B'性状。因此，它还需要实现'A'性状。如果程式没有实现'A'性状，则Rust编译器会丢掷错误。
