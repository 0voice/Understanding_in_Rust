# Rust可恢复的错误

可恢复的错误是那些完全停止程式并不严重的错误。可以处理的错误称为可恢复错误。它由 结果
`Result <T，E>` `<T，E>` `OK <T>` `Err <E>`

```
OK <T>`：'T'是一种值，它在成功情况下时返回 ：'E'是一种错误，它在失败情况下时返回`OK`
`Err <E>``ERR
Enum Result<T,E>  
{  
    OK<T>,  
    Err<E>,  
}
```

- 在上面的例子中，`Result` `OK <T>＆Err <E>` `'T'` `'E'`
- `'T'`是一种值，它将在成功的情况下返回，而`'E'`
- `Result`包含泛型型别引数，因此在成功和失败值可能不同的许多不同情况下使用标准库中定义的结果型别和函式。

下面来看一个返回`Result`

```rust
use std::fs::File;  
 fn main()   
{  
     let f:u32 = File::open("vector.txt");  
}
```

执行上面范例程式码，得到以下结果 -

![img](https://tw511.com/upload/images/201910/20191014013940399.png)

在上面的范例中，Rust编译器显示该型别不匹配。是 上面的输出显示成功值的型别是`'f'` `u32` `File::open` `Result <T，E>` `std::fs::File` `std::io::Error`

**注意：**

- `File::open`返回型别是成功值或失败值。如果 结果列举提供此资讯。`File::open` `File::open`
- 如果`File::open` `f` `OK` `File::open` `Err`

## 匹配表示式以处理结果变体

下面来看看一个匹配表示式的简单范例：

```c
use std::fs::File;  
fn main()  
{  
   let f = File::open("vector.txt");  
   match f   
   {  
       Ok(file) => file,  
       Err(error) => {  
       panic!("There was a problem opening the file: {:?}", error)  
     },  
   }; 
}
```

执行上面范例程式码，得到以下结果 -

![img](https://tw511.com/upload/images/201910/20191014013940400.png)

**程式说明**

- 在上面的范例中，可以直接存取列举变体，而无需在`OK` `Err` `Result::`
- 如果结果正常，则返回档案并将其储存在 在匹配之后，可以在档案中执行读取或写入操作。`'f'`
- 匹配对 如果`Err` `Result` `Error` `panic!`

#### 出错时Error:unwrap()

- 结果 其中一种方法是 方法是匹配表示式的快捷方法。方法和匹配表示式的工作方式是一样的。`<T，E>``unwrap()``unwrap()``unwrap()`
- 如果`Result` `OK` `unwrap()` `OK`
- 如果`Result` `Err` `unwrap()` `panic!`

下面来看一个简单的范例：

```rust
use std::fs::File;  

fn main()  
{  
     File::open("hello.txt").unwrap();  
}
```

执行上面范例程式码，得到以下结果：

![img](https://tw511.com/upload/images/201910/20191014013940401.png)

在上面的例子中，`unwrap()` `panic!`

#### Error: expect()

- `expect()`方法的行为方式与`unwrap()` `panic!`
- `expect()`和 因此，可以说`unwrap()` `expect()` `unwrap()` `expect()` `panic!`

下面看看一个简单范例 -

```shell
use std::fs::File;  
fn main()  
{  
     File::open("hello.txt").expect("Not able to find the file hello.txt");  
}
```

执行上面范例程式码，得到以下结果 -

![img](https://tw511.com/upload/images/201910/20191014013940402.png)

在上面的输出中，错误讯息显示在程式中指定的输出萤幕上，即 如果包含多个`「無法找到檔案hello.txt」` `unwrap()` `unwrap()` `panic!`

## 传播错误

传播错误是一种将错误从一个函式转发到另一个函式的机制。错误传播到呼叫函式，其中有更多资讯可用，以便可以处理错误。假设有一个名为 想要建立一个程式来读取档案，先参考下面一个简单的例子：

```rust
use std::io;  
use std::io::Read;  
use std::fs::File;  
fn main()  
{  
  let a = read_username_from_file();  
  print!("{:?}",a);  
}  
fn read_username_from_file() -> Result<String, io::Error>   
{  
    let f = File::open("a.txt");  
    let mut f = match f {  
    Ok(file) => file,  
    Err(e) => return Err(e),  
    };  
    let mut s = String::new();  
    match f.read_to_string(&mut s) {  
        Ok(_) => Ok(s),  
        Err(e) => Err(e),  
    }  
}
```

程式说明 -

- `read_username_from_file()`函式返回`Result <T，E>` `'T'` `String` `'E'` `io` `Error`
- 如果函式成功，则返回一个包含`String` `OK` `Err`
- 函式中首先呼叫 如果`File::open` `File::open` `Err` `File::open``f`
- 如果 如果`File::open` `String` `read_to_string()`
- 假设我们有一个名为 因此，该程式读取档案

#### 传播错误的捷径：`?`

使用 运算子是匹配表示式的替换意味着 假设有一个名为 想要建立一个程式来对该档案执行读取操作。`?` `?` `?` `「yiibai」`

看看下面一个简单的例子。

```c
use std::io;  
use std::io::Read;  
use std::fs::File;  
fn main()  
{  
  let a = read_username_from_file();  
  print!("{:?}",a);  
}  
fn read_username_from_file() -> Result<String, io::Error>   
{  
   let mut f = File::open("a.txt")?;  
   let mut s = String::new();  
   f.read_to_string(&mut s)?;  
  Ok(s)  
}
```

在上面的例子中，如果`?` `Result` `Result` `OK` `OK` `Result` `Err`

#### ?运算子和匹配表示式的区别

- 使用`?` `from trait`
- 当`?`
- 如果没有错误发生，那么`?` `OK` `Err`
- 它使函式的实现更简单。

#### 链方法在？运算子之后呼叫

甚至可以通过在`?`

下面来看一个简单的例子：

```rust
use std::io;  
use std::io::Read;  
use std::fs::File;  
fn main()  
{  
  let a = read_username_from_file();  
  print!("{:?}",a);  
}  
fn read_username_from_file() -> Result<String, io::Error>   
{  
    let mut s = String::new();  
   File::open("a.txt")?.read_to_string(&mut s)?;  
   Ok(s)  
}
```

**程式说明**

在上面的例子中，将 如果两个函式(即`read_to_string()` `File::open("a.txt")?` `read_to_string()` `File::open("a.txt")` `OK`

#### ?运算子的限制

`?`运算子只能在返回 运算子与匹配表示式的工作方式类似。匹配表示式仅适用于`Result` `?` `Result`

下面通过一个简单的例子来理解这一点。

```rust
use std::fs::File;  
fn main()   
{  
    let f = File::open("a.txt")?;  
}
```
