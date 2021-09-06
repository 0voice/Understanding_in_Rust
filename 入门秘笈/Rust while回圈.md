# Rust while回圈

`while-loop`是一个条件回圈。当程式需要评估条件时，则使用条件回圈。当条件为真时，它执行回圈，否则它终止回圈。

**while回圈的语法**

```
while condition  
//block statements;
```

在上面的语法中，如果条件为真，则执行块语句，否则终止回圈。Rust提供了这个内建构造，可以与`while``loop``if``else``break`

**while回圈流程图**

![img](https://tw511.com/upload/images/201910/20191014013910377.png)

下面来看一个简单的例子 -

```rust
 fn main()  
{  
  let mut i=1;  
  while i<=10  
    {  
       print!("{}", i);  
       print!(" ");  
       i=i+1;  
    }  
}
```

执行上面范例程式码，得到以下输出结果 -

```
1 2 3 4 5 6 7 8 9 10
```

在上面的例子中，回圈执行直到`i``i``while``i``10``10`

下面来看一个简单的例子

```rust
fn main()  
{  
  let array=[10,20,30,40,50,60];  
  let mut i=0;  
  while i<6  
  {  
    print!("{}",array[i]);  
    print!(" ");  
    i=i+1;  
  }  
}
```

输出结果 -

```
10 20 30 40 50 60
```

在上面的范例中，使用`while`

`while`回圈的缺点：

- 如果索引长度不正确，回圈可能会导致问题。
- 当编译器新增执行时程式码以通过此回圈对每次叠代执行条件检查时，它也很慢。
