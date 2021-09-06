# Rust开发环境安装

在学习Rust之前。首先，需要安装Rust，通过 `rustup`

## Windows上Rust安装

在Windows上，开启连结 按照所有说明操作后，将安装Rust并显示萤幕：`rustup-init.exe`

![img](https://tw511.com/upload/images/201910/20191014013900370.png)



接着回车 -

![img](https://tw511.com/upload/images/201910/20191014013900371.png)



然后开始下载并安装Rust 环境。

安装后，Rust的PATH变数会自动新增到系统PATH中。开启命令提示字元然后执行以下命令：

```shell
$ rustc --version
```

执行此命令后，应该看到版本号，提交的杂凑值和提交日期。如果看到类似的结果，则表示Rust已成功安装。

结果如下所示 -

```
C:\Users\hema>rustc --version
rustc 1.30.0 (da5f414c2 2018-10-24)
```

> 注意：使用C++工具安装visual studio是执行rust程式的必要条件。

## Linux或macOS中的Rust安装

如果使用的是Linux或macOS，请开启终端然后使用以下命令：

```shell
$ curl https://sh.rustup.rs -sSf | sh
```

上面的命令下载指令码并开始安装Rust工具，它将安装最新版本的Rust。如果安装成功完成，则会显示以下讯息：

```shell
Rust is installed now. Great!
```

下次登入后，此安装会自动将Rust新增到系统路径中。如果要立即执行Rust而不重新启动终端，请执行以下命令到`shell`

```shell
$ source $HOME/.cargo/env
```

安装后，需要一个连结器。当尝试执行Rust程式时，将收到连结器无法执行的错误。这意味着系统中未安装连结器。C编译器总是提出正确的编译器。安装C编译器。另外，一些Rust包依赖于C程式码，需要一个C编译器。

## 更新和解除安装

**更新：执行以下命令以更新到最新版本：**

```shell
$ rustup update
```

**解除安装：**

```shell
$ rustup self uninstall
```
