# Rust if语句

```
if`语句确定条件是否为真。如果条件为`true``if``if
```

表示`if`

- if块
- if-else块
- if else-if阶梯块
- 巢状if语句

## if语句

`if`语句块的语法 -

```rust
if condition  
{  
    //block statements;  
}
```

在上面的语法中，如果条件为真，则执行块语句，否则跳过`if`

`if`语句的流程图 -

![img](https://tw511.com/upload/images/201910/20191014013903372.png)

**范例：**
`if`

```rust
fn main(){

 let a=1;  
 if a==1  
 {  
      println!("a is equal to 1");  
 }
}
```

执行上面范例程式码，得到以下结果：

```
a is equal to 1
```

在这个例子中，因此，`a``1``if``println!`

## if-else语句

如果条件为真，则执行 如果条件为假，则跳过`if``else``if``else`

**if-else语句的语法**

```
if condition  
{  
   //block statements  
}else{  
    //block statements  
}
```

**if-else的流程图**

![img](https://tw511.com/upload/images/201910/20191014013903373.png)

下面来看看一个`if-else`

```rust
fn main()  
{  
  let a=3;  
  let b=4;  
  if a>b  
  {  
     println!("a is greater than b");  
  }  
  else  
   {  
     println!("a is smaller than b");   
   }  
}
```

执行上面范例程式码，得到以下结果 -

```
a is smaller than b
```

在该范例中，变数 因此，执行`a``3``a``b``else`

## else-if语句

如果要检查多个条件，则可使用`else-if`

`else-if`语句的语法 -

```
if condition 1  
{  
  //block statements  
}else if condition 2  
{  
  //block statements  
}   
.  
.  
else{  
//block statements  
}
```

在上面的语法中，Rust为第一个真实条件执行块，当匹配到第一个真条件时，它就不会执行其余的块。

`else if`语句块的流程图 -

![img](https://tw511.com/upload/images/201910/20191014013903374.png)

下面来看一个`else-if`

```rust
fn main(){

 let num= -5;  
 if num>0  
 {  
   println!("number is greater than 0");  
 }  
 else if num<0  
 {  
   println!("number is less than 0 ");  
 }  
 else  
 {  
   println!("number is not equal to 0");  
 }
}
```

执行上面范例程式码，得到以下结果 -

```shell
number is less than 0
```

在此范例中，变数 因此，`num``-5``num``0``else if`

## 巢状if-else语句

当 巢状`if-else``if``else``if-else`
`if-else`

```rust
if condition 1  
{  
   // 巢狀if/else塊  
   if condition 2  
    {  
         //block statements  
    }else  
    {  
        //block statements  
    }  
}else{  
   //block statements  
}
```

下面来看一个巢状`if-else`

```rust
fn main(){

 let a=5;  
 let b=6;  
 if a!=b  
 {  
   if a>b  
   {  
     println!("a is greater than b");  
   }else{  
      println!("a is less than b");  
   }  
 }  

 else  
 {  
      println!("a is equal to b");  
 }
}
```

执行上面范例程式码，得到以下结果 -

```shell
a is less than b
```

在此范例中，因此，控制进入 因此，执行`a``b``if``a``b``else``if`
