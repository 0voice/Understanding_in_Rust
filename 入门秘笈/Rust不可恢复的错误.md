# Rust不可恢复的错误

不可恢复的错误是检测到的错误，程式员无法处理它。当发生这种错误时，列印失败讯息。清理堆叠然后退出。`panic!``panic!``panic!`

![img](https://tw511.com/upload/images/201910/20191014013938396.png)

**展开(Unwinding) 但是，展开过程需要大量工作。的替代方案是 中止(Aborting) 作业系统将删除资料。如果从展开切换到中止，那么需要新增以下语句：**`Unwinding` `Aborting`

```rust
panic = 'abort';
```

下面来看一个`panic!`

```rust
fn main()  
{
   panic!(?No such file exist?);
}
```

执行上面范例程式码，得到如下结果 -

![img](https://tw511.com/upload/images/201910/20191014013938397.png)

在上面的输出中，第一行显示错误讯息，它传达两个资讯，即 讯息是「没有这样的档案存在」 和 `panic` `panic` `error.rs:3:5`

> 注意：一般来说，不实现`panic!` `panic!`

## panic!的好处

Rust语言没有缓冲区重读问题。缓冲区重写是一种情况，当从缓冲区读取资料并且程式超出缓冲区时，即它读取相邻的储存器。这导致违反记忆体安全。

下面来看一个简单的例子：

```rust
fn main()  
{  
   let v = vec![20,30,40];  
   print!("element of a vector is :",v[5]);  
}
```

执行上面范例程式码，得到以下结果 -

![img](https://tw511.com/upload/images/201910/20191014013938398.png)



在上面的例子中，试图存取索引 在这种情况下，Rust会因为存取无效索引而引发 因此，Rust不会返回任何内容。但是，对于其他语言(如C和C++)，它们会返回一些内容，尽管该向量不属于该记忆体。这称为缓冲区重写，它会导致安全问题。`5` `panic`

**Rust回溯 需要设定**
`RUST_BACKTRACE`
