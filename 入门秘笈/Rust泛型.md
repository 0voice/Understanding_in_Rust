# Rust泛型

当要建立多种形式的功能时，即，函式的引数可以接受多种型别的资料。这可以通过泛型来实现。泛型也称为「引数多型」，其中多型是多重的，而变形是形式。

有两种方法可以提供通用程式码：

- `Option<T>`
- `Result<T, E>`

![img](https://tw511.com/upload/images/201910/20191014013943403.png)

1. 它提供了一种型别的泛型。`Option<T>` `Option` `'T'`

```rust
enum Option<T>  
{  
    Some(T),  
    None,  
}
```

在上面的例子中，可以用任何资料型别替换 下面来看看这几个范例：`enum` `<T>` `T`

```rust
let x : Option<i32> = Some(10);  // 'T' is of type i32.  
let x : Option<bool> = Some(true);  // 'T' is of type bool.  
let x : Option<f64> = Some(10.5); // 'T' is of type f64.  
let x : Option<char> = Some('b'); // 'T' is of type char.
```

在上面的例子中，观察到 但是，如果左侧的型别与右侧的值不匹配，则会发生错误。如下范例：`'T'` `i32` `bool` `f64` `char`

```rust
let x : Option<i32> = Some(10.8);
```

在上述情况下，左侧的型别是 因此，错误发生「型别不匹配」。`i32` `f64`

1. `Result <T,E>`： Rust标准库提供了另一种资料型别`Result <T，E>` `T＆E`

```rust
enum Result<T,E>  
   {  
      OK(T),  
        Err(E),  
}
```

> 注意：不得不使用`'T'` `'E'`

#### 泛型函式

泛型可以在函式中使用，将泛型放在函式的签名中，其中指定引数的资料型别和返回值。

- 当函式包含型别为`T`

**语法**

```rust
fn function_name<T>(x:T)   
// body of the function.
```

上面的语法包含两部分：

- `<T>` : 给定的函式是一种型别的泛型。
- `(x : T)`: x 是型别`T`

当函式包含多个相同型别的引数时。

```rust
fn function_name<T>(x:T, y:T)   
// body of the function.
```

当函式包含多个型别的引数时。

```rust
fn function_name<T,U>(x:T, y:U)  
// Body of the function.
```

完整程式码 -

```rust
 fn main()  
{  
  let a = vec![1,2,3,4,5];  
  let b = vec![2.3,3.3,4.3,5.3];  
  let result = add(&a);  
  let result1 = add(&b);  
  println!("The value of result is {}",result);  
  println!("The value of result1 is {}",result1);  
}  

fn add<T>(list:&[T])->T  
{  
  let mut c =0;  
  for &item in list.iter()  
  {  
    c= c+item;  
  }  
}
```

## 结构定义

结构也可以使用`<>`

**语法：**

```rust
struct structure_name<T>   
// Body of the structure.
```

在上面的语法中，在`struct_name` `struct`

下面我们来看一个简单的例子：

```rust
struct Value<T>  
{  
  a:T,  
  b:T,  
}  
fn main()  
{  
  let integer = Value{a:2,b:3};  
  let float = Value{a:7.8,b:12.3};  
  println!("integer values : {},{}",integer.a,integer.b);  
  println!("Float values :{},{}",float.a,float.b);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
integer values : 2,3
Float values : 7.8,12.3
```

在上面的范例中，建立两个范例 包含`Value <T>` `a` `b` `integer` `float` `Integer` `i32` `float` `f64`

下面来看另一个简单的例子。

```rust
struct Value<T>  
{  
  a:T,  
  b:T,  
}  
fn main()  
{  
  let c = Value{a:2,b:3.6};  
  println!("c values : {},{}",c.a,c.b);  
}
```

执行上面范例程式码，得到以下结果：



![img](https://tw511.com/upload/images/201910/20191014013943404.png)

在上面的范例中，建立了一个 包含不同型别的值，即 因此，Rust编译器会丢掷「不匹配的错误」。`Value <T>` `a` `b` `c` `c` `i32` `f64`

## 列举定义

列举也可以使用通用资料型别。Rust标准库提供了 是一个列举，其中`Option <T>` `Option <T>` `T`

- `Option<T>`

它由两个变体组成，即`Some(T)` `None`

![img](https://tw511.com/upload/images/201910/20191014013943405.png)

其中`Some(T)` `T` `None`

看看下面一段范例程式码：

```rust
enum Option<T>  
{  
    Some(T),  
    None,  
}
```

在上面的例子中，它由两个变体`Option` `T` `Some(T)` `None`

```
Result<T, E>`：可以建立多种型别的泛型，这可以通过`Result <T，E>
enum Result<T,E>  
{  
    OK(T),  
    Err(E),  
}
```

在上面的例子中，`Result <T，E>` `OK(T)` `Err(E)`

`OK(T)`保持型别`T` `Err(E)` `E`

## 方法定义

可以在结构和列举上实现这些方法。下来看看一个简单的例子：

```rust
struct Program<T> {  
    a: T,  
    b: T,  
}  
impl<T> Program<T>   
{  
    fn a(&self) -> &T   
{  
       &self.a  
    }  
}

fn main() {  
    let p = Program{ a: 5, b: 10 };  

    println!("p.a() is {}", p.a());  
}
```

输出结果如下 -

```shell
p.a() is 5
```

在上面的例子中，在 在`Program <T>` `a` `a` `impl` `T` `Program <T>`

## 解决歧义

Rust编译器自动推断通用引数。下面通过一个简单的场景来理解：

```rust
Let mut v = Vec::new();   // creating a vector.  
v.push(10); // inserts integer value into the vector. Therefore, v is of i32 type.  
println!("{:?}", v); // prints the value of v.
```

在上面的例子中，将整数值插入向量中。因此，Rust编译器知道向量`v``i32`

如果删除第二行，现在程式码如下所示 -

```rust
Let mut v = Vec::new();   // creating a vector.  
println!("{:?}", v); // prints the value of v.
```

上面的情况将丢掷「它无法推断出T的型别」的错误。

可以通过两种方式解决上述问题：

1. 使用以下注释：

```rust
let v : Vec<bool> = Vec::new();  
println!("{:?}",v) ;
```

2. 使用`'turbofish':: <>``'T'`

```rust
let v = Vec :: <bool> :: new();  
println!("{:?}",v) ;
```
