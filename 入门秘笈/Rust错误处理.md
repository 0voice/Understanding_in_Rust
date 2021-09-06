# Rust错误处理

错误处理是Rust确定出错的可能性并确认在程式码进行编译之前采取某些操作的机制。此机制使程式更加健壮，因为能够在部署生产程式码之前发现并处理错误。Rust程式设计语言不包含异常。

Rust中有两种型别的错误：

- 不可恢复的错误。
- 可恢复的错误。

![img](https://tw511.com/upload/images/201910/20191014013935392.png)

- **可恢复的错误：完全停止该过程的可恢复错误并不严重。它由 可恢复错误的范例是「找不到档案」。是通用引数。这是一种值，在成功的情况下返回一个'OK'变数。这是一种错误型别，在具有**`Result <T，E>``T＆E`
  `T->`
  `E->``Err`
- **不可恢复的错误：例如：「除以零」是不可恢复错误的范例。**`!`

#### 可恢复错误与不可恢复错误

可恢复错误是可以某种方式恢复的错误，而不可恢复错误是无法以任何方式恢复的错误。下面来看一下预期行为的情景：

```
"100".parse();
```

在上述情况下，因此，它是一个可恢复的错误。`"100"`

**意外的行为**

![img](https://tw511.com/upload/images/201910/20191014013935393.png)

**assert! 如果它不正确和错误，则程式停止执行。**

下面来看一个简单的例子：

```rust
fn main()  
{  
    let x : bool = false;  
    assert!(x==true);  
}
```

执行上面范例程式码，得到以下结果：

![img](https://tw511.com/upload/images/201910/20191014013935394.png)

在上面的例子中，因此，在执行时`x` `false` `assert!` `assert!` `panic!`

**unreachable! 此巨集很有用，因为编译器无法确定无法存取的程式码。在执行时由**

下面来看一个简单的例子：

```rust
enum Value  
{  
  Val,  
}  

fn get_number(_:Value)->i32  
{   
   5  
}  
fn find_number(val:Value)-> &'static str  
{  
  match get_number(val)  
  {  
    7 => "seven",  
    8=> "eight",  
    _=> unreachable!()  
  }  
}  

fn main()  
{  
  println!("{}", find_number(Value::Val));  
}
```

执行上面范例程式码，得到以下结果 -

![img](https://tw511.com/upload/images/201910/20191014013936395.png)

在上面的范例中，因此，`get_number()` `5` `unreachable!` `panic!`
