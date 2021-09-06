# Rust第一个程式

在本文中，使用Rust语言编写简单的程式，以了解如何编写，储存和编译Rust程式。现在，开启记事本档案并编写以下程式码：

```rs
fn main(){
    println!("Hello, world!");
}
```

将上面内容储存到一个档案：`rustc hello.rs`

```shell
Hello, world!
```

- `main()`：函式用大括号 函式不包含任何引数，也不返回任何值。`main()``main()``{}``main()`
- `println!`：这是一个Rust巨集。如果它呼叫该函式，则它不包含符号：`'!'`
- `"Hello World"`：它是作为引数传递给`println!`

## 建立，编译和执行程式的过程

1. 开启记事本档案并将程式码写入记事本档案中。
2. 使用`.rs`
3. 开启命令提示字元
4. 设定目录的路径，假设专案位于`/home/hema/worsp/rust`
5. 使用`rustc`
6. 最后，使用命令`./filename`

```shell
hema@yiibai:~/worsp/rust$ rustc hello.rs && ./hello
Hello World!
```

> 注：如果有遇到「error: could not exec the linker`link.exe`
