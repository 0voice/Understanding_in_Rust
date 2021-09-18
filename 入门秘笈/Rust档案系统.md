# Rust档案系统

------

模组形成层次结构，使专案变得更容易理解。Rust模组系统用于分割多个档案，使得并非所有内容都位于`src/lib.rs` `src/main.rs`

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

在这种情况下，不需要像在 并且，如果在这里编写`mod` `mod` `A`

Rust预设情况下会检视`src/lib.rs`

现在，从档案`src/lib.rs` `B` `B`

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

现在建立包含模组 外部档案的名称将命名为- 建立档案后，在此档案中写入先前已删除的模组`B` `src/B.rs` `B`

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

现在将从档案`src/B.rs` `C` `C`

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

> 注意：从模组B中提取模组C将导致编译错误，因为 因此，`src/B.rs` `src/lib.rs` `src/B.rs` `src/B/mod.rs` `B`

**模组档案系统规则：**

- 如果模组名为「server」且没有子模组，则模组的所有宣告都可以放在档案`server.rs`
- 如果名为「server」的模组包含子模组，则模组的所有宣告都将放在档案`server/mod.rs`
