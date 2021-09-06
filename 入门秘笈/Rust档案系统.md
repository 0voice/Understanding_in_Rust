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

模组形成层次结构，使专案变得更容易理解。Rust模组系统用于分割多个档案，使得并非所有内容都位于`src/lib.rs``src/main.rs`

档案名：

```rust
mod A  
{  
     fn a()  
     {  
          // block of statements.  
     }  
}    
mod B  
{  
     fn b()  
     {  
            // block of statements.    
     }  
   mod C  
  {  
       fn c()  
       {  
             // block of statements.  
       }  
  }    
}
```

在上面的例子中，程式由三个模组组成，即 是`A``B``C``C``B`

给定档案的模组层次结构是：

![img](https://tw511.com/upload/images/201910/20191014013928388.png)

如果模组包含许多函式并且函式非常冗长，则很难找到特定函式的程式码。Rust通过提供模组系统提供了灵活性。可以拥有每个模组的单独档案，而不是放在同一个档案中，即`src/lib.rs`

**要遵循的步骤：**
`A`

```rust
mod A;  
mod B  
{  
     fn b()  
     {  
            // block of statements.    
     }  
     mod C  
    {  
       fn c()  
       {  
             // block of statements.  
       }  
     }    
}
```

分号`;``A``A`

**模组A;**

```rust
mod A  
{  
     fn a()  
     {  
          // block of statements.  
     }  
}
```

现在建立包含模组A定义的外部档案。外部档案的名称将命名为- 建立档案后，在此档案中写入模组A的定义，该档案先前已被删除。

档案名：

```rust
fn a()  
    // block of statements.
```

在这种情况下，不需要像在 并且，如果在这里编写`mod``mod``A`

Rust预设情况下会检视`src/lib.rs`

现在，从档案`src/lib.rs``B``B`

档案名：

```rust
mod A;  
mod B;
```

**mod B;**

```rust
mod B  

    fn b()  
    {  
           // block of statements.    
    }  
  mod C  
 {  
      fn c()  
      {  
            // block of statements.  
      }  
 }
```

现在建立包含模组 外部档案的名称将命名为- 建立档案后，在此档案中写入先前已删除的模组`B``src/B.rs``B`

档案名：`src/B.rs`

```rust
fn b()  
    {  
           // block of statements.    
    }  
      mod C  
     {  
          fn c()  
          {  
                // block of statements.  
          }  
     }
```

现在将从档案`src/B.rs``C``C`

```rust
fn b()  
     {  
            // block of statements.    
     }  
mod C;
```

**mod C;**

```rust
mod C  
{  
     fn c()  
     {  
           // block of statements.  
     }  
}
```

现在建立包含模组 外部档案的名称将命名为 建立档案后，在此档案中写入模组`C``src/C.rs``C`

档案名称:

```rust
fn c()  
      {  
            // block of statements.  
      }
```

> 注意：从模组B中提取模组C将导致编译错误，因为 因此，`src/B.rs``src/lib.rs``src/B.rs``src/B/mod.rs``B`

**模组档案系统规则：**

- 如果模组名为「server」且没有子模组，则模组的所有宣告都可以放在档案`server.rs`
- 如果名为「server」的模组包含子模组，则模组的所有宣告都将放在档案`server/mod.rs`
