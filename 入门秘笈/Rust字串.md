# Rust字串

Rust包含两种型别的字串：`&str` `String`

**String**

- 字串被编码为UTF-8序列。
- 在堆记忆体上分配一个字串。
- 字串的大小可以增长。
- 它不是以空(`null`

**&str**

- `&str`也称为字串切片。
- 它由`&[u8]`
- `＆str`用于检视字串中的资料。
- 它的大小是固定的，即它不能调整大小。

**String 和&str 的区别**

- `String`是一个可变参照，而`&str` `String` `&str`
- `String`包含其资料的所有权，而`&str`

## 建立一个新的字串

在建立向量时类似地建立`String`

建立一个空字串：

```rust
Let mut s = String::new();
```

在上面的宣告中，现在，如果想在宣告时初始化String，可以通过使用`String` `new()` `to_string()`

在资料上实现`to_string()`

```rust
let a = "Yiibai";  
let s = a.to_string();
```

也可以直接在字串文字上实现`to_string`

```rust
let s = "Yiibai".to_string();
```

下面通过一个例子来理解这一点：

```rust
fn main()  
{
 let data="Yiibai";  
 let s=data.to_string();  
 print!("{} ",s);  
 let str="tutorial".to_string();  
 print!("{}",str);
}
```

执行上面范例程式码，得到以下结果 -

```shell
Yiibai tutorial
```

建立 下面通过一个简单的例子来理解这一点：`String``String::from``String::new()`

```rust
fn main()  
{  
    let str = String::from("Yiibai tutorial");  
    print!("{}",str);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Yiibai tutorial
```

## 更新字串

可以通过将更多资料推播到 也可以使用格式巨集的`String``String``String``+`

![img](https://tw511.com/upload/images/201910/20191014013934391.png)

使用 它将内容附加在字串的末尾。假设`push_str`  `push` `push_str()` `push_str()` `s1` `s2` `s3` `s4`

```rust
s1.push_str(s2);
```

通过一个简单的例子来理解这一点：

```rust
fn main()  
{  
  let mut s=String::from("java is a");  
  s.push_str(" programming language");  
  print!("{}",s);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
java is a programming language
```

`push_str()`函式不接受引数的所有权。下面通过一个简单的例子来理解。

```rust
fn main()  
{  
  let mut s1 = String::from("Hello");  
  let s2 = "World";  
  s1.push_str(s2);  
  print!("{}",s2);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
World
```

如果`push_str()` `s2`

`push()`：假设字串是`push()` `s1 ` `ch` `s1`

```
s1.push(ch);
```

下面来看一个简单的范例

```rust
fn main()  
{  
  let mut s = String::from("java");  
  s.push('c');  
  print!("{}",s);  
}
```

执行上面范例程式码，得到以下结果-

```shell
javac
```

- 使用 下面来看一个范例程式码：`+` `+` `+`

```rust
let s1 = String::from("Yiibai ");  
let s2 = String::from("tutorial!!");  
let s3 = s1+&s2;
```

再来看看一个简单的程式码：

```rust
fn main()  
{  
 let s1 = String::from("Yiibai");  
 let s2 = String::from(" tutorial!!");  
 let s3 = s1+&s2;   
 print!("{}",s3);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Yiibai tutorial!!
```

在上面的例子中，不再有效，使用 运算子呼叫`s3` `"Yiibai tutorial!!"` `s1` `s2` `&s2` `+` `+` `add()`

```rust
fn add(self,s:&str)->String  
{  
}
```

首先，根据 但是根据 但是，仍然可以在 因此，当呼叫`s2` `&` `s1` `add()` `&str` `String` `add()` `s2` `&String` `&str` `add` `s2` `&string` `&str` `add()`

其次，这意味着在语句`add()` `self` `add()` `self` `let s3 = s1 +&s2` `s1`

下面通过一个简单的例子来理解这一点：

```rust
fn main()  
{  
 let s1 = String::from("C");  
 let s2 = String::from("is");  
 let s3 = String::from("a");  
 let s4 = String::from("programming");  
 let s5 = String::from("language.");  
 let s = format!("{} {} {} {} {}",s1,s2,s3,s4,s5);  
 print!("{}",s);  
}
```

执行上面范例程式码，得到以下结果：

```shell
C is a programming language.
```

## 字串中的索引

`String`以 因此，字串无法编入索引。下面通过一个例子来理解这个概念：`UTF-8`

```
fn main()   
{  
    let s = String::from("Yiibai");  
    print!("{}",s[1]);  
}
```

执行上面范例程式码，得到类似以下的结果 -

```shell
error[E0277]: the trait bound `std::string::String: std::ops::Index<{integer}>` is not satisfied
 --> jdoodle.rs:4:17
  |
4 |     print!("{}",s[1]);
  |                 ^^^^ the type `std::string::String` cannot be indexed by `{integer}`
  |
  = help: the trait `std::ops::Index<{integer}>` is not implemented for `std::string::String`

error: aborting due to previous error
```

通过索引存取非常快。但是，字串以`UTF-8``n`

## 字串切片

字串中未提供索引，因为不知道索引操作的返回型别应具有位元组值，字元或字串切片。Rust提供了一种更具体的方法来索引字串，方法是在`[]`

**范例：**

```rust
let s = "Hello World";  
let a = &s[1..4];
```

在上面的场景中，这里指定`s` `"Hello World"` `[1..4]` `1` `3`

```rust
fn main() {  

    let s = "Hello World";  
    let a = &s[1..4];  
    print!("{}",a);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
ell
```

## 叠代字串的方法

也可以通过其他方式存取字串。使用`chars()`

下面来看一个简单的例子：

```
fn main()   
{  
    let s = "C is a programming language";  
    for i in s.chars()  
    {  
      print!("{}",i);  
    }  
}
```

执行上面范例程式码，得到以下结果 -

```
C is a programming language
```
