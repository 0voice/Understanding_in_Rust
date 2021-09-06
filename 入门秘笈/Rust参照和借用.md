# Rust参照和借用

参照是作为引数传递给函式的地址。借用就像我们借一些东西，如果已经完成借用，需要还给原所有者。参照和借用是相互的，即当参照被释放时，借用也结束。

## 为什么要借用？

使用借用概念的原因如下：

- 借用允许对单个资源进行多次参照，但仍然遵守「单一所有者」。
- 参照就像C中的指标一样。
- 参照是一个物件。参照有两种型别，即可变参照和不可变参照。在复制不可变参照时移动可变参照。

下面通过一个例子来理解这一点。

```rust
 fn main()  
{  
 let str=String::from("Yiibai");  
 let len=calculate_length(&str);  
 println!("length of the string {}",len);  
}  
fn calculate_length(s:&String)->usize  
{  
  s.len()  
}
```

执行上面范例程式码，得到以下结果 -

```
length of the string 6
```

在上面的范例中，`calculate_length()``str`

```rust
let str=String::from("Yiibai");  
let len=calculate_length(&str);
```

在上面的场景中，因此，即使参照超出范围，也不会删除参照指向的值。`&str``str`

```rust
fn calculate_length(s:&String)->usize  
s.len()
```

在上面的例子中，变数 当变数作为函式的参照而不是实际值传递时，不需要返回值到返回所有权。`s``main()`

下面尝试修改借用的值。

```rust
fn main()  
{  
 let x=1;  
 value_changed(&x)  
}  
fn value_changed(y:&i32)  
{  
 *y=9;  
}
```

以下是上述程式的输出：

![img](https://tw511.com/upload/images/201910/20191014013915384.png)

在上面的范例中，它会引发错误，因为 因此，无法改变`&x``y`

## 可变参照

可以通过使用可变参照来修复上述错误。可变参照是那些可以改变的参照。下面通过一个例子来理解这一点。

```rust
fn main()  
{  
 let mut x=1;  
 value_changed(&mut x);  
 println!("After modifying, the value of x is {}",x);  
}  
fn value_changed(y:&mut i32)  
{  
 *y=9;  
}
```

执行上面范例程式码，得到以下结果 -

```shell
After modifying, the value of x is 9
```

在上面的例子中，建立了一个可变参照，即 现在，可以更改 分配 因此，`&mut x``y``&i32``y``9``* y = 9``x``9`

## 可变参照的限制

只能对特定范围内的一段资料进行一次可变参照。例如：

```rust
let mut str=String::from("Yiibai");  
let a= &mut str;  
let b= &mut str;
```

在上面的场景中，编译器丢掷一个错误，因为它包含两个在Rust语言中不可能的可变参照。如果程式中存在不可变参照，那么程式中就不能有可变参照。例如：

```rust
let mut str=String::from("Yiibai");  
let a= &str;  
let b=&str;  
let c=&mut str;
```

在上面的场景中，编译器丢掷一个错误，因为当有一个不可变参照时，不能有一个可变参照。
