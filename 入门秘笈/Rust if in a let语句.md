# Rust if in a let语句

在`let``if``if``let`

**if in a let语法**

```rust
Let variable_name= if condition{  
 //code blocks  
}else{  
 //code block  
}
```

在上面的语法中，如果条件为真，则将`if``false``else`

![img](https://tw511.com/upload/images/201910/20191014013905375.png)

**范例1**

下面来看一个简单的例子。

```rust
fn main(){

 let a=if true  
       {  
          1  
       }  
       else  
       {  
           2  
       };  
 println!("value of a is: {}", a);
}
```

执行上面范例程式码，得到以下结果 -

```shell
value of a is: 1
```

在此范例中，条件为真。因此，现在，`a``if``a``1`

下面再来看一个另一个简单的例子。

```rust
fn main(){

 let a=if false  
       {  
          9  
       }  
       else  
       {  
           "yiibai"  
       };  
 println!("value of a is: {}", a);
}
```

执行上面范例程式码，得到以下结果 -

```
Some errors occurred:E0308
```

在此范例中，因此，该程式丢掷错误，因为两个块都包含不同型别的值。`if``else`
