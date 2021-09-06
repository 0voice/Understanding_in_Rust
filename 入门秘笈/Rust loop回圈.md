# Rust loop回圈

如果想要多次执行语句块，那么回圈概念就属于这个角色。回圈执行回圈体记忆体在的程式码直到结束，并从启动开始立即重新开始。

Rust有三种回圈：

- loop回圈
- for回圈
- while回圈

## loop回圈

`loop`不是条件回圈。它是一个关键字，告诉Rust一次又一次地执行程式码块，直到除非明确地手动停止回圈。

**loop回圈**

```rust
loop{  
  //block statements  
}
```

在上面的语法中，块语句被无限次执行。

回圈流程图：

![img](https://tw511.com/upload/images/201910/20191014013907376.png)

下面来看看一个无限回圈的简单例子 -

```
fn main(){
     loop  
     {  
         println!("Hello Yiibai");  
    }
}
```

执行上面范例程式码，得到以下结果 -

```
Hello Yiibai
Hello Yiibai
Hello Yiibai
Hello Yiibai
.
.
.
infinite times
```

在这个例子中，「Hello Yiibai」字串一遍又一遍地列印，直到除非手动停止回圈。通常，「ctrl + c」命令用于从回圈终止。

#### 回圈终止

```
break`关键字用于从回圈终止。如果未使用`break
```

下面来看一个简单的例子 -

```rust
fn main()  

 let mut i=1;  
 loop  
 {
       println!("Hello Yiibai");  
       if i==7   
       {  
         break;  
       }  
     i+=1;  
 }
}
```

执行上面范例程式码，得到以下结果 -

```shell
Hello Yiibai
Hello Yiibai
Hello Yiibai
Hello Yiibai
Hello Yiibai
Hello Yiibai
Hello Yiibai
```

在上面的例子中，`i`
