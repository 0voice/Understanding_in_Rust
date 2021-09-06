# Rust use关键字参照模组

当呼叫模组的函式时，需要指定完整的路径。

通过下面一个例子来理解这个概念：

```rust
pub mod a  
{  
  pub mod b  
  {  
    pub mod c  
    {  
      pub fn nested_modules()  
      {  
        println!("Nested Modules");  
      }  
    }  
  }  
 }  

fn main()  
{  
 a::b::c::nested_modules();  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Nested Modules
```

在上面的例子中，通过指定完整路径来呼叫`nested_modules()``a::b::c::nested_modules()`

## use关键字

在上面的场景中，看到函式呼叫非常冗长。Rust中的 关键字只在范围中指定的那些模组。通过下面一个例子来理解这一点：`use``use`

```rust
pub mod a  
{  
  pub mod b  
  {  
    pub mod c  
    {  
      pub fn nested_modules()  
      {  
        println!("Nested Modules");  
      }  
    }  
  }  
 }  

use a::b::c::nested_modules;  
fn main()  
{  
  nested_modules();  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Nested Modules
```

在上面的范例中，因此，可以直接呼叫函式，而不必在呼叫函式中包含模组。`use`

列举也是模组之类的名称空间的一种形式。因此，可以使用 在`use``use`

通过下面一个例子来理解：

```rust
#[derive(Debug)]  
enum Flagcolor  
{  
 Orange,  
 White,  
 Green,  
}  
use Flagcolor::{Orange,White,Green};  
fn main()  
{  
  let _o= Orange;  
  let _w= White;  
  let _g= Green;  
  println!("{:?}",_o);  
  println!("{:?}",_w);  
  println!("{:?}",_g);  
}
```

执行上面范例程式码，得到以下结果：

```shell
orange
white
green
```

在上面的范例中，因此，可以直接使用列举变体而不使用列举名称和名称空间说明符。`Flagcolor``use`

## 使用* 运算子

```
*`运算子用于将所有专案放入范围，这也称为 如果使用`glob``glob
```

通过下面一个例子来理解这一点：

```rust
#[derive(Debug)]  
enum Color  
{  
  Red,  
  Yellow,  
  Green,  
  Orange,  
}  

use Color::*;  
fn main()  
{  
  let _red=Red;  
  let _yellow=Yellow;  
  let _green=Green;  
  let _orange=Orange;  
  println!("{:?}",_red);  
  println!("{:?}",_yellow);   
  println!("{:?}",_green);  
  println!("{:?}",_orange);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Red
Yellow
Green
Orange
```

在上面的范例中，`*``use`

## 使用super 关键字

`super`关键字用于从当前模组存取父模组，它使能够存取父模组的私有功能。

```rust
mod a{  
    fn x() -> u8 {  
        5  
    }  

    pub mod example {  
        use super::x;  

        pub fn foo() {  
            println!("{}",x());  
        }  
    }
}  

fn main()  
{  
  a::example::foo();  
}
```

输出结果如下 -

```shell
2
```

在上面的范例中，模组范例使用了参照其父模组的 由于这个原因，模组范例的`super``foo()``a`
