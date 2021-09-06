# Rust模组

模组是一个名称空间，包含函式或其型别的定义。模组是函式，结构，特征，预设情况下，模组的修饰符是私有的，但可以使用`impl``pub``public`

以下是模组中使用的关键字：

- **mod关键字**`mod`
- **pub关键字 关键字使可见性修饰符成为公共，因此，它们可在名称空间外部存取。**`pub`
- **use关键字**`use`

## 模组定义

模组由`mod`

模组的语法：

```rust
mod module_name  
// body inside the module.
```

模组可以通过三种方式分类：

**1.单个模组：**

通过下面一个例子来理解这一点：

```rust
mod a  
{  
     pub fn single_module()  
    {  
      println!("Single module");  
    }  
}  
fn main()  
{  
  a::single_module();  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Single module
```

在上面的范例中，定义了一个模组- 可以使用模组名称后跟名称空间然后使用函式名称来呼叫模组`a``a``a`

也可以使用单独的档案来执行上面的范例：

```rust
mod module;  
fn main()  
{  
  module::single_module();  
}
pub fn single_module()  
{  
    println!("Single module");  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Single module
```

在上面两个例子中，检查`mod X``X.rs``X/mod.rs`

**2.子模组：假设库名称是-**`language``C``Cplus`

下面给出了`language`

![img](https://tw511.com/upload/images/201910/20191014013926387.png)

通过下面一个例子来理解：

```rust
mod c  
{  
  pub fn c()  
  {  
    println!("C is a structured programming language");  
  }  
}  
mod cplus  
{  
 pub fn cplus()  
 {  
    println!("C++ is an object-oriented programming language");  
 }  
}  
fn main()  
{  
  c::c();  
  cplus::cplus();  
}
```

执行上面范例程式码，得到以下结果：

```shell
C is a structured programming language
C++ is an object-oriented programming language
```

在上面的例子中，程式由两个模组组成，即`c``cplus``c::c()``cplus::cplus()`

**3.巢状模组：**

通过下面一个例子来理解这一点：

```rust
mod a  
{  
 pub fn a()  
 {  
   println!("a module");  
 }  
 pub mod b  
 {  
   pub fn a()  
   {  
     println!("b module");  
   }  
 }  
}  
fn main()  
{  
 a::a();  
 a::b::b();  
}
```

执行上面范例程式码，得到以下结果 -

```shell
a module
b module
```

在上面的例子中，程式由两个模组组成，即 这两个模组都包含具有相同名称但功能不同。这两个函式分别使用 它们都不会相互冲突，因为它们属于不同的名称空间。`a``b``b``a``a::a()``a::b::b()`
