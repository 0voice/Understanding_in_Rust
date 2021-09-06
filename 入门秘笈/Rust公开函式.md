# Rust公开函式

`pub`关键字用于宣告的开头，以便外部函式可以存取该函式。

**以下是私有规则：**

- 如果任何函式或模组是公共的，则任何父模组都可以存取它。
- 如果任何函式或模组是私有的，则可以通过其直接父模组或父项的子模组来存取它。
- 通过下面一个简单的例子来理解这一点：

```rust
mod outer  
{  
   pub fn a()  
   {  
     println!("function a");          
   }  
   fn b()  
   {  
      println!("function b");  
   }  

mod inner  
{  
  pub fn c()  
  {  
    println!("function c");  
  }  
  fn d()  
  {  
    println!("function d");  
  }  
}  
}  
fn main()  
{  
  outer::a();  
  outer::b();  
  outer::inner::c();  
  outer::inner::d();  
}
```

执行上面范例程式码，得到以下结果 -

![img](https://tw511.com/upload/images/201910/20191014013929389.png)

在上面的范例中，因此，`main()``outer``main()``outer`

函式`a()``outer::a()``main()``outer::b()`

```
main()`函式无法存取内部模组，因为它是私有的。模组没有子模组，因此只能由其父模组(即`inner``outer
```
