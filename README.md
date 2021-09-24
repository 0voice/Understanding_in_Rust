# 🏄💨【最安全的编程语言】Rust工程师枕边资料，大牛文章，开源框架，官方文档，视频，推荐书籍，学习干货，大牛语录

<div align=center>

![rust](https://user-images.githubusercontent.com/87457873/132184451-55f1125e-acad-4cc7-9e56-ecbffc0db412.png)
  
## 一个安全、并发、实用的系统语言

<br>
<br>
  
   [🏝<br>&nbsp;&nbsp;&nbsp; &nbsp;环境搭建&nbsp;&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E7%8E%AF%E5%A2%83%E6%90%AD%E5%BB%BA)  |[📕<br>&nbsp;&nbsp;&nbsp; 入门秘笈&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88-pdf%E6%A1%A3%E4%B8%8B%E8%BD%BD)|  [📖<br>&nbsp;&nbsp;&nbsp; 推荐书籍&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E6%8E%A8%E8%8D%90%E4%B9%A6%E7%B1%8D)
:-------: | :-------: | :---------:
 **[📑<br>精选文章](https://github.com/0voice/Understanding_in_Rust#-%E5%A4%A7%E7%89%9B%E6%96%87%E7%AB%A0)**  |  **[📰<br>官方文档](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E5%AE%98%E6%96%B9%E6%96%87%E6%A1%A3)**|  **[✈<br> 杂货铺](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E6%9D%82%E8%B4%A7%E9%93%BA)**
**[💽<br>视频](https://github.com/0voice/Understanding_in_Rust#-%E8%A7%86%E9%A2%91)** | **[🏗<br>开源框架](https://github.com/0voice/Understanding_in_Rust#-%E5%BC%80%E6%BA%90%E6%A1%86%E6%9E%B6)** | **[🐂<br>大牛语录](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E5%A4%A7%E7%89%9B%E8%AF%AD%E5%BD%95)**
  
<br>
<br>  

</div>




# 🤔 Why Rust？Why can？

### Jay Oster, PubNub 架构师 :

“除了安全和性能，我们还有：

- 泛型；
- 特征；
- 代数类型；
- 函数式和命令式范式；
- 可能是世界上最好的依赖管理和构建工具，实际上解决了‘依赖地狱’问题；
- 对内嵌文档、测试和性能评测的美妙支持；
- 一个大的且正在生长的库、抽象、工具生态；
- 过程宏；
- 与已有代码的 FFI 交互性；
- 支持一打平台（更多的在路上！）；
- 对开发者体验是正向的、毋庸置疑的满足。

Rust 是唯一一个下面所有框框都打勾的语言：

- 内存安全
- 类型安全
- 消除数据竞争
- 使用前编译
- 建立（并且鼓励）在零抽象之上
- 最小的运行时（无停止世界的垃圾搜集器，无 JIT 编译器，无 VM）
- 低内存占用（程序可以运行在资源受限的环境，比如小的微控制器）
- 裸金属目标（比如，写一个 OS 内核或者设备驱动，把 Rust 当一个 ‘高层’汇编器使用）”

### Peter Varo:

“Rust 有一个很香的地方：它像 C 和 C++ 那样底层，因此也具有底层的这些优势（比如，控制、大小、速度等）。同时呢，它又像 Haskell 那样高层，自带令人吃惊的大量功能传承。它还是命令式的，所以容易被大多数人上手。然后它又像 Python 一样灵活，比如，' 鸭子类型（duck-typing）' 的概念出现在编译时（比如，特征限定），然后它又没有陈旧的面向对象模型以及由这个模型导致的各种出名的问题。

最后但很重要的是，还有一连串的东西被包含进来：精简短小的语法，语言提供的数目不多的特性，标准库及其一致性，高质量的文档的集成，包括对初学者和高级用户都适用的学习材料，这些都是促成因素。”

# 🏝 环境搭建

**安装及工具：https://www.rust-lang.org/zh-CN/learn/get-started**

# 📕 入门秘笈 [（PDF档下载）](https://github.com/0voice/Understanding_in_Rust/blob/main/Rust%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88.pdf)

- [Rust简介](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%AE%80%E4%BB%8B.md)<br>
- [Rust的特点](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%9A%84%E7%89%B9%E7%82%B9.md)<br>
- [Rust开发环境安装](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83%E5%AE%89%E8%A3%85.md)<br>
- [Rust第一个程式](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%AC%AC%E4%B8%80%E4%B8%AA%E7%A8%8B%E5%BC%8F.md)<br>
- [Rust if语句](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20if%E8%AF%AD%E5%8F%A5.md)<br>
- [Rust if in a let语句](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20if%20in%20a%20let%E8%AF%AD%E5%8F%A5.md)<br>
- [Rust loop回圈](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20loop%E5%9B%9E%E5%9C%88.md)<br>
- [Rust for回圈](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20for%E5%9B%9E%E5%9C%88.md)<br>
- [Rust while回圈](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20while%E5%9B%9E%E5%9C%88.md)<br>
- [Rust所有权](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%89%80%E6%9C%89%E6%9D%83.md)<br>
- [Rust参照和借用](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%8F%82%E7%85%A7%E5%92%8C%E5%80%9F%E7%94%A8.md)<br>
- [Rust切片](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%88%87%E7%89%87.md)<br>
- [Rust结构体](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%BB%93%E6%9E%84%E4%BD%93.md)<br>
- [Rust结构体更新语法](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%BB%93%E6%9E%84%E4%BD%93%E6%9B%B4%E6%96%B0%E8%AF%AD%E6%B3%95.md)<br>
- [Rust结构体方法语法](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%BB%93%E6%9E%84%E4%BD%93%E6%96%B9%E6%B3%95%E8%AF%AD%E6%B3%95.md)<br>
- [Rust列举](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%88%97%E4%B8%BE.md)<br>
- [匹配运算子](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/%E5%8C%B9%E9%85%8D%E8%BF%90%E7%AE%97%E5%AD%90.md)<br>
- [Rust if let控制流程](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20if%20let%E6%8E%A7%E5%88%B6%E6%B5%81%E7%A8%8B.md)<br>
- [Rust模组](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%A8%A1%E7%BB%84.md)<br>
- [Rust档案系统](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%A1%A3%E6%A1%88%E7%B3%BB%E7%BB%9F.md)<br>
- [Rust公开函式](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%85%AC%E5%BC%80%E5%87%BD%E5%BC%8F.md)<br>
- [Rust use关键字参照模组](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20use%E5%85%B3%E9%94%AE%E5%AD%97%E5%8F%82%E7%85%A7%E6%A8%A1%E7%BB%84.md)<br>
- [Rust向量](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%90%91%E9%87%8F.md)<br>
- [Rust字串](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%AD%97%E4%B8%B2.md)<br>
- [Rust错误处理](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E9%94%99%E8%AF%AF%E5%A4%84%E7%90%86.md)
- [Rust不可恢复的错误](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E4%B8%8D%E5%8F%AF%E6%81%A2%E5%A4%8D%E7%9A%84%E9%94%99%E8%AF%AF.md)<br>
- [Rust可恢复的错误](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%8F%AF%E6%81%A2%E5%A4%8D%E7%9A%84%E9%94%99%E8%AF%AF.md)<br>
- [Rust泛型](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%B3%9B%E5%9E%8B.md)<br>
- [Rust Trait](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Trait.md)<br>
- [Rust生命周期](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F.md)<br>
- [Rust智慧指标](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%99%BA%E6%85%A7%E6%8C%87%E6%A0%87.md)<br>
- [Rust Box<T>](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Box%3CT%3E.md)<br>
- [Rust Deref trait](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Deref%20trait.md)<br>
- [Rust Drop trait](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Drop%20trait.md)<br>

# 📖 推荐书籍
  
### 国内书籍
  
- [《深入浅出Rust》](https://jp1lib.org/s/?q=%E3%80%8A%E6%B7%B1%E5%85%A5%E6%B5%85%E5%87%BARust%E3%80%8B)
  
- [《Rust权威指南》](https://book.douban.com/subject/35081743/)
  
- [《Rust 程序设计语言》](https://kaisery.github.io/trpl-zh-cn/)
  
- [《精通Rust(第2版)》](https://jp1lib.org/book/17127064/820864)
  
### 国外书籍
  
**入门书籍**
  
- [《The Rust Programming Language》](https://doc.rust-lang.org/book/)
  
欢迎！本书将教你有关 Rust 编程语言的知识。Rust 是一种系统编程语言，专注于三个目标：安全性、速度和并发性。它在没有垃圾收集器的情况下实现了这些目标，使其成为其他语言不擅长的许多用例的有用语言：嵌入其他语言、具有特定空间和时间要求的程序以及编写低级代码，例如设备驱动程序和操作系统。它通过在不产生运行时开销的情况下进行大量编译时安全检查，同时消除所有数据竞争，从而改进了针对此空间的当前语言。Rust 还旨在实现“零成本抽象”，尽管其中一些抽象感觉像是高级语言的抽象。即便如此，Rust 仍然允许像低级语言一样进行精确控制。
  
- [《Welcome to Rust-101》](https://www.ralfj.de/projects/rust-101/main.html)
  
这是 Rust-101，一个 Rust 语言的小教程。它旨在成为一门交互式的动手课程：我相信真正学习一门语言的唯一方法是在其中编写代码，因此您应该在课程中进行编码。如果您有任何未在此处回答的问题，请查看下面的“其他资源”。尤其是，IRC 频道里挤满了愿意帮助你的很棒的人！我在那里花了很多时间 ;-) 我假设对编程有一定的了解，因此不会解释大多数语言共有的基本概念。相反，我将专注于 Rust 的特殊之处。
  
- [《Rust by Example》](http://rustbyexample.com/)
  
Rust by Example (RBE) 是一组可运行的示例，用于说明各种 Rust 概念和标准库。
  
- [《Why Rust?》](https://kr1lib.org/book/10990507/3a18af) 
  
尽管自 40 多年前引入 C 以来，系统编程语言已经有了很大的发展，但我们对造成巨大后果的愚蠢错误的能力仍然没有改变，新闻中经常有生动的例子。这份 O'Reilly 报告研究了 Rust，这是一种新的系统编程语言，它将安全性和安全性与性能相结合，与 C 和 C++ 相当。
  
- [《Learning Rust》](https://kr1lib.org/book/11689651/08c0b6) 
  
Rust 是一种高度并发和高性能的语言，专注于安全和速度、内存管理和编写干净的代码。它还保证线程安全，其目的是提高现有应用程序的性能。它得到了 Mozilla 的支持，以解决并发的关键问题。 
  
- [《Beginning Rust - From Novice to Professional》](https://kr1lib.org/book/3490555/7b7c82)
  
学习在 Unix、Linux shell、macOS 和 Windows 命令行上以简单、循序渐进的方式使用 Rust 进行编程。当您阅读本书时，您将建立在您在前几章中获得的知识的基础上，并了解 Rust 提供了什么。

开始 Rust 从 Rust 的基础开始，包括如何命名对象、控制执行流和处理原始类型。您将看到如何进行算术运算、分配内存、使用迭代器以及处理输入/输出。一旦掌握了这些核心技能，您将着手处理错误并使用 Rust 的面向对象特性立即构建健壮的 Rust 应用程序。

只需要基本的编程知识，最好是 C 或 C++。要理解这本书，知道什么是整数和浮点数，以及区分标识符和字符串文字就足够了。
  
- [《Rust Cookbook》](https://kr1lib.org/book/3362654/66eb5a)  
  
本书将帮助您理解 Rust 语言的核心概念，使您能够通过整合零成本抽象和更好的内存管理等功能来开发高效和高性能的应用程序。深入研究 Rust 中的高级概念，例如错误处理、宏、包和并行性。在本书的最后，学习如何创建 HTTP 服务器和 Web 服务，在服务器端编程方面建立强大的基础知识，并能够提供使用 Rust 构建高性能和更安全的生产级 Web 应用程序和服务的解决方案。
  
- [《Rust Standard Library Cookbook》](https://kr1lib.org/book/3571952/9b9cdb)  
  
Mozilla 的 Rust 以其惊人的功能和强大的库而备受关注。本书将带您了解各种秘诀，教您如何利用标准库来实现高效的解决方案。

本书首先简要介绍了标准库和馆藏的基本模块。从这里开始，食谱将涵盖通过解析支持文件/目录处理和交互的包。您将了解与高级数据结构、错误处理和网络相关的包。您还将学习使用期货和实验性夜间功能。这本书还涵盖了 Rust 中最相关的外部 crate。
  
- [《Network Programming with Rust》](https://kr1lib.org/book/3571947/48c564)  
  
Rust 足够低级，可以提供对内存的细粒度控制，同时通过编译时验证提供安全性。这使得它特别适合编写低级网络应用程序。

本书分为三个主要部分，将带您踏上构建功能齐全的 Web 服务器的激动人心的旅程。本书首先对 Rust 和基本的网络概念进行了扎实的介绍。这将为整本书奠定基础并定下基调。在第二部分中，我们将深入研究如何使用 Rust 开发网络软件。从使用套接字的客户端-服务器网络到 IPv4/v6、DNS、TCP、UDP，您还将了解使用 serde 序列化和反序列化数据。这本书展示了如何通过 HTTP 与 REST 服务器进行通信。本书的最后一部分讨论了使用 Tokio 堆栈进行异步网络编程。鉴于安全对于现代系统的重要性，您将看到 Rust 如何支持常见的原语，例如 TLS 和公钥加密。
  
- [《Rust Programming by Example》](https://kr1lib.org/book/5669466/ef3a67) 
  
从介绍 Rust 开始，您将学习基本方面，例如其语法、数据类型、函数、泛型、控制流等。在此之后，您将直接开始构建您的第一个项目，俄罗斯方块游戏。接下来，您将使用 Tokio（可扩展且高效的异步 IO Rust 库）构建图形音乐播放器并使用快速、可靠的网络软件。

在本书的过程中，您将探索 Rust 编程的各种特性，包括它的 SDL 特性、事件循环、文件 I/O 和著名的 GTK+ 小部件工具包。通过这些项目，您将看到 Rust 在并发方面的表现——包括并行性、可靠性、改进的性能、泛型、宏和线程安全。我们还将介绍 Rust 的一些异步和反应式编程方面。
  
- [《Rust Quick Start Guide》](https://kr1lib.org/book/11689628/cf06fb)
  
熟悉使用流行的新系统编程语言编写程序，这些语言将低级语言的强大性能与多线程代码中的线程安全等高级功能结合在一起。
  
- [《Rust in Action [MEAP]》](https://kr1lib.org/book/11235796/a7ef40)  
  
Rust in Action 是一本面向想要探索 Rust 编程语言世界的中级程序员的书。它适用于可能已经用尽网络上的免费资料但仍想了解更多信息的人。它与 Rust 编程的其他材料不同，因为它还教您有关系统编程的知识。您将能够更多地了解 CPU 的工作原理、计算机如何计时、指针是什么以及您的网卡和键盘如何告诉 CPU 它们已准备好读取输入。

从系统编程书籍的角度来看，它实际上也是独一无二的 - 因为几乎每个示例都适用于 Windows！如果你是那种喜欢实际例子的学习者，你会喜欢阅读这本书。
  
- [《A Gentle Introduction to Rust》](https://stevedonovan.github.io/rust-gentle-intro/)  
  
Rust 是一种静态和强类型的系统编程语言。静态意味着所有类型在编译时都是已知的，强烈意味着这些类型旨在使编写不正确的程序变得更加困难。一个成功的编译意味着你可以比使用像 C 这样的牛仔语言更好地保证正确性。系统意味着生成最好的机器代码，并完全控制内存使用。因此，其用途非常核心：操作系统、设备驱动程序和甚至可能没有操作系统的嵌入式系统。然而，它实际上也是一种非常令人愉快的语言，可以用来编写普通的应用程序代码。

与 C 和 C++ 的最大区别在于 Rust 默认是安全的；检查所有内存访问。意外损坏内存是不可能的。
  
- [《Practical Machine Learning with Rust: Creating Intelligent Applications in Rust》](https://kr1lib.org/book/5304256/0ff807)  
  
Rust 中的机器学习已经被社区忽视了很长一段时间。由于宇宙中散布着许多不同的板条箱，这本书试图统一所有的信息和用法，并在某种程度上动摇社区采取行动。数据是新的前沿领域，而 Rust 必须成为其中的一部分。

阅读了使用 Rust 的实用机器学习之后，您将对使用 Rust 创建高计算库有一个深入的了解。掌握了这种神奇语言的知识，您将能够创建性能更高、内存安全且资源占用更少的应用程序。
  
- [《Rust Web Development》](https://kr1lib.org/book/11729741/a127f0)  

Rust Web Development 是使用 Rust 构建基于服务器的 Web 应用程序的实践指南。如果您使用 Java、C# 或 PHP 构建了 Web 服务器，您会立即爱上 Rust 提供的性能和开发体验。本书向您展示了如何使用纯 Rust 以及重要的 Rust 库（例如用于异步运行时的 tokio、用于 Web 服务器和 API 的 warp 以及运行外部 HTTP 请求的 reqwest 等）高效工作。

您可以将这本书交给新聘用的开发人员，并让他们使用这本书。它包含非常实用的示例和模式，并为未来探索该主题奠定了坚实的基础。
  
**进阶书籍**
 
- [《The Rustonomicon》](https://doc.rust-lang.org/nightly/nomicon/)
  
本书深入探讨了编写正确的不安全 Rust 程序所需的所有可怕细节。由于这个问题的性质，它可能会导致释放出无法言喻的恐怖，将你的心灵粉碎成十亿个无限小的绝望碎片。

如果您希望编写 Rust 程序的职业生涯长久而快乐，那么现在您应该回过头来忘记您曾经看过这本书。这不是必要的。但是，如果您打算编写不安全的代码——或者只是想深入了解语言的本质——这本书包含了宝贵的信息。  
  
- [《Programming Rust》](https://1lib.limited/book/3400043/791885) 
  
这本实用的书向系统程序员介绍了 Rust，一种新的前沿语言。您将了解 Rust 如何提供静态验证的内存安全和低级控制的罕见且有价值的组合——想象一下 C++，但没有悬空指针、空指针取消引用、泄漏或缓冲区溢出。  
  
- [《Rust Essentials - Second Edition》](https://1lib.limited/book/3427870/81d715)  
  
本书首先论证了 Rust 在当今编程语言领域的独特地位。安装 Rust 并学习如何使用它的包管理器 Cargo。逐步介绍各种概念：变量、类型、函数和控制结构，以打下基础。然后探索更多结构化数据，例如字符串、数组和枚举，并了解模式匹配的工作原理。

在这一切中，本书强调了 Rust 编译器用来生成安全代码的独特推理方式。接下来看看 Rust 特定的错误处理方式，以及特征在 Rust 代码中的整体重要性。在我们探索各种指针类型时，将深入探讨内存安全的支柱。接下来，看看宏如何简化代码生成，以及如何使用模块和板条箱组合更大的项目。最后，了解我们如何在 Rust 中编写安全的并发代码并与 C 程序接口，了解 Rust 生态系统，并探索标准库的使用。  
  
- [《Hands-On Concurrency with Rust》](https://1lib.limited/book/11689707/4154e1)  
  
本书将教你如何在现代机器上管理程序性能，并在 Rust 中构建快速、内存安全和并发的软件。它从 Rust 的基础开始，讨论机器架构概念。您将了解如何系统地衡量和改进 Rust 代码的性能，以及如何自信地编写集合。您将了解应用于线程的 Sync 和 Send 特性，并使用锁、原子原语、数据并行等来协调线程执行。

本书将向您展示如何在 C++ 代码中有效地嵌入 Rust，并探索用于多线程应用程序的各种 crate 的功能。它深入探讨了实现。您将了解互斥锁的工作原理并自行构建多个互斥锁。您将掌握生态系统中存在的完全不同的方法来构建和管理大规模系统。
  
- [《Hands-On Functional Programming in Rust》](https://1lib.limited/book/11689735/4d162e)
  
函数式编程允许开发人员将程序划分为更小的、可重用的组件，从整体上简化软件的创建、测试和维护。结合 Rust 的强大功能，您可以开发满足现代软件需求的强大且可扩展的应用程序。本书将帮助您发现可用于以功能方式构建软件的所有 Rust 功能。

我们首先对针对不同问题和模式的函数式方法和面向对象方法进行简要比较。然后我们快速查看控制流的模式、数据以及这些函数式编程独有的抽象。下一部分介绍如何在 Rust 中创建功能性应用程序；还讨论了 Rust 独有的可变性和所有权。接下来检查纯函数，您将掌握闭包、它们的各种类型和柯里化。我们还通过功能设计原则和使用宏的元编程来实现并发。最后，我们看看调试和优化的最佳实践。

读完本书，您将熟悉函数式编程方法，并能够在日常工作中使用这些技术。  
  
- [《Rust High Performance》](https://1lib.limited/book/11000538/3e9291)
  
有时，很难从 Rust 中获得最佳性能。这本书教你将你的 Rust 代码的速度优化到 C/C++ 等语言的水平。您将了解并修复常见的陷阱，了解如何通过使用元编程来提高生产力，并通过安全轻松地并发执行部分代码来加速代码。您将掌握这门语言的特性，这将使您脱颖而出，并使用它们来真正提高算法的效率

本书以一个温和的介绍开始，以帮助您识别 Rust 编程时的瓶颈。我们重点介绍了常见的性能缺陷，以及及早发现和解决这些问题的策略。我们继续掌握 Rust 的类型系统，这将使我们能够在编译时在性能和安全性方面进行令人印象深刻的优化。然后，您将学习如何在 Rust 中有效地管理内存，掌握借用检查器。我们继续测量性能，您将看到这如何影响您编写代码的方式。继续前进，您将在 Rust 中执行元编程，以提高代码的性能和生产力。您最终将学习 Rust 中的并行编程，它通过使用多线程和异步编程实现高效和更快的执行。
  
- [《Zero To Production In Rust》](https://zero2prod.com/) 
  
如果您想学习如何使用 Rust 进行后端开发，这里就是您的最佳选择。

Rust 的采用率达到了历史最高水平：越来越多的公司正在尝试和招聘。<br>
如果您对使用 Rust 构建 API 感兴趣，零到生产是您 Rust 之旅的理想起点。<br>
您将边做边学：我们将从头开始，一步一步地构建一个功能齐全的电子邮件通讯后端 API。<br>

您将学习：

1、导航和利用 Rust 的 crates 生态系统<br>
2、构建您的应用程序以使其模块化和可扩展<br>
3、编写测试，从单个单元到成熟的集成测试<br>
4、使用类型系统为您的域建模以强制执行不变量<br>
5、收集日志、跟踪和指标以观察应用程序的状态<br>
6、为您的 Rust 项目设置一个强大的持续集成和持续部署管道<br>
  
- [《Programming WebAssembly with Rust》](https://1lib.limited/book/5001228/7b21a9)  
  
WebAssembly 不仅仅是一项革命性的新技术。它正在重塑我们为 Web 及其他领域构建应用程序的方式。在 ActiveX 和 Flash 等技术失败的地方，您现在可以使用您喜欢的任何语言编写代码并编译为 WebAssembly，以便在浏览器、移动设备、嵌入式设备等中运行的快速、类型安全的代码。将 WebAssembly 的便携、高性能模块与 Rust 的安全性和强大功能相结合，是一个完美的开发组合。

了解 WebAssembly 的堆栈机器架构如何工作，安装低级 wasm 工具，并发现编写原始废弃代码的黑暗艺术。在此基础上构建并学习如何通过实现跳棋游戏的逻辑从 Rust 编译 WebAssembly 模块。在 Rust 中创建 wasm 模块，以多种引人注目的方式与 JavaScript 进行互操作。将您的新技能应用于非网络主机的世界，并创建从在 Raspberry Pi 上运行的控制照明系统的应用程序到功能齐全的在线多人游戏引擎，开发人员可以上传他们自己的竞技场绑定 WebAssembly 战斗模块.

立即开始使用 WebAssembly，并改变您对 Web 的看法。  
  
- [《Step Ahead with Rust: Systems Programming in Rust》](https://www.armstrong-publications.com/product/step-ahead-with-rust-super-combo/)  
  
从基本的编程模式到深入了解该语言，Step Ahead with Rust 旨在帮助您从编写程序到使用 Rust 构建软件。本书将向您展示 Rust 语言最重要的特性，包括货物、类型系统、迭代器等。读完本书，您应该会熟悉更多内容，并准备好处理其余的高级主题。

在您阅读本书的过程中，我们建议您花时间尝试一下书页中所呈现的内容。这本书都是关于 Rust 的实际应用，所以在实践中应用它是值得期待的。本书涵盖：货物、Rust 类型系统、迭代器、宏、所有权、借用和生命周期、不安全模式、并发。A Step Ahead with Rust 读者应该是一位经验丰富的开发人员，希望提高他们的 Rust 开发技能。  
  
- [《Creative Projects for Rust Programmers》](https://1lib.limited/book/5639719/c52aca)  
  
了解 Rust 编程语言的最新特性、有用的库和框架的实用指南，将帮助您设计和开发有趣的项目

学习：

1、访问 TOML、JSON 和 XML 文件以及 SQLite、PostgreSQL 和 Redis 数据库<br>
2、使用 JSON 有效负载开发 RESTful Web 服务<br>
3、使用 HTML 模板和 JavaScript 创建 Web 应用程序，使用 WebAssembly 创建前端 Web 应用程序或 Web 游戏<br>
4、构建桌面 2D 游戏<br>
5、为编程语言开发解释器和编译器<br>
6、创建机器语言模拟器<br>
7、使用可加载模块扩展 Linux 内核<br>
  
# 📑 大牛文章
  
- [理解 Rust 的生命周期](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E7%90%86%E8%A7%A3%20Rust%20%E7%9A%84%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F.md)
- [高德技术 | 基于Rust的Android Native内存分析方案](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E5%9F%BA%E4%BA%8ERust%E7%9A%84Android%20Native%E5%86%85%E5%AD%98%E5%88%86%E6%9E%90%E6%96%B9%E6%A1%88.md)
- [Rust 与 C++：深入的语言比较](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/Rust%20%E4%B8%8E%20C%2B%2B%EF%BC%9A%E6%B7%B1%E5%85%A5%E7%9A%84%E8%AF%AD%E8%A8%80%E6%AF%94%E8%BE%83.md)
  
# 📰 官方文档
  
- [标准库API文档](https://doc.rust-lang.org/std/)
- [Rust Reference](https://doc.rust-lang.org/reference/index.html): Rust reference 文档，有中文翻译版本 [Rust语言规范](https://rustlang-cn.org/office/rust/reference/) 正在翻译过程中
- [Rust编译错误索引](https://doc.rust-lang.org/error-index.html)：发生编译错误时，可以通过索引找到具体错误解释
- [rustdoc文档](https://doc.rust-lang.org/rustdoc/): `restdoc`工具的使用文档
- [Rustonomicon](https://doc.rust-lang.org/reference/): rust的参考文档。但是目前并不完整，可能有遗漏和错误
- [Unstable Book](https://doc.rust-lang.org/unstable-book/): 用于尚不稳定特性的文档
- [Rustonomicon](https://doc.rust-lang.org/nomicon/): unsafe rust的黑暗艺术，有中文翻译版本 [Rust高级编程](https://rustlang-cn.org/office/rust/advrust/)
- [The Cargo Book](https://doc.rust-lang.org/cargo/index.html): cargo使用介绍，有中文翻译版本 [Cargo教程](https://rustlang-cn.org/office/rust/cargo/) 正在进行中
- [Rust Edition Guide](https://doc.rust-lang.org/nightly/edition-guide/introduction.html): Rust 版本指南，传递 Rust 不同版本之间大的变更信息
- [Command line apps in Rust](https://rust-lang-nursery.github.io/cli-wg/#command-line-apps-in-rust): 在Rust中编写命令行程序
  
# ✈ 杂货铺
  
- Rust 最大中文社区论坛：https://rustcc.cn/
- 小众中文社区的翻译资料/论坛：https://learnku.com/rust
- Rust在线编辑器: https://play.rust-lang.org/
- 2021 年去哪学 Rust：https://loige.co/where-to-go-to-learn-rust-in-2021/
- Rust Cheat Sheet（Rust语法备忘单）：https://cheats.rs/
- Rust 中文书架与资讯：https://budshome.com/ | https://blog.budshome.com/
- 简要而基础的 Rust 知识（适合在 Rust Book 阶段当作补充材料）：https://learning-rust.github.io/
- 微软发布的 Rust 新手教程：https://docs.microsoft.com/en-us/learn/paths/rust-first-steps/
- Rust-leetcodes刷题：https://stevenbai.top/rust-leetcode/
- Rust by Example 通过例子学 Rust：https://doc.rust-lang.org/rust-by-example/index.html
- 电子书下载 ：https://jp1lib.org/s/Rust
- Rust线下全球会议：
  - RustConf: https://rustconf.com/
  - Rust Belt Rust: https://rust-belt-rust.com/
  - RustFest: https://blog.rustfest.eu/
  - Rust Latam: https://rustcon.asia/
  - RustCon Asia: https://rustcon.asia/
  
# 💽 视频
  
Rust 验证研讨会 2021 | 
:------:|
[Peeking at compiler-internal data (for fun and profit)](https://www.aliyundrive.com/s/4N4EE3URbBT)|
[Ferrite- A Rust EDSL for Message-passing Protocol Verification](https://www.aliyundrive.com/s/hGpvaNzWAHS)|
[Verifying that Rust programs don't crash](https://www.aliyundrive.com/s/TiMG3B7XXyZ)|
[crux-mir- Symbolic testing for Rust](https://www.aliyundrive.com/s/j5LG8Lwdmx8)|
[RustBelt- A Quick Dive Into the Abyss](https://www.aliyundrive.com/s/iv3ohCTjzcs)|
[Rustv- Semi-automatic Verification of Unsafe Rust Programs](https://www.aliyundrive.com/s/bfQjMdJTvow)|  
[Polonius](https://www.aliyundrive.com/s/bNdQLDpKbzN)|
[Towards Automatic Verification of Unsafe Rust with Constrained Horn Solvers](https://www.aliyundrive.com/s/iW2SdR1pFGU)|
[Rust interest in safety- and mission-critical environments](https://www.aliyundrive.com/s/EXnsFymhCib)|  
[Prusti – Deductive Verification for Rust](https://www.aliyundrive.com/s/eph1UzJugSt)|
[Creusot- A prototype tool for verification of Rust software](https://www.aliyundrive.com/s/6aeaQNeGZbX)|
[hacspec_ succinct, executable, verifiable specifications for high-assurance cryptography](https://www.aliyundrive.com/s/DgfNNFRn45G)|  
[Leveraging Compiler Intermediate Representation for Multi- and Cross-Language Verification](https://www.aliyundrive.com/s/oWuWB37ByBH)|
  
<br>
  
Rust Linz 2021 | 
:------:|
[Rust Linz, July 2021 - Stefan Baumgartner - Serverless Rust](https://www.aliyundrive.com/s/7nBT4iWyT5p)|  
[Rust Linz, July 2021 - Rainer Stropek - Traits, not your grandparents' interfaces](https://www.aliyundrive.com/s/1fSbir945Sh)|
[Rust Linz, August 2021 - Rainer Stropek - Rust iterators](https://www.aliyundrive.com/s/G3Yu2U7DaXN)|  
[Rust Linz, May 2021 - Harald Reingruber - Rust for Medical Visualization](https://www.aliyundrive.com/s/5u27AdX5bhq)|  
[Rust Linz, May 2021 - Lisa Passing - Creative Rust](https://www.aliyundrive.com/s/WouXfuZ9VSU)|  
[Rust Linz, June 2021 - Tim McNamara - How to learn Rust](https://www.aliyundrive.com/s/XhSexAWPNKr)|  
[Rust Linz, June 2021 - JT - A new path for your shell](https://www.aliyundrive.com/s/cymDeWwbsr6)|
[Rust Linz x Global Azure, April 2021 - Ryan Levick & Thomas Taylor - Rust, Kubernetes, and the Cloud](https://www.aliyundrive.com/s/Gdd63ojU9Xc)|  
[Rust Linz, April 2021 - Jan-Erik Rediger - Leveraging Rust to build cross-platform libraries](https://www.aliyundrive.com/s/rfPAYT9NWi9)|  
[Rust Linz, April 2021 - Herbert Wolverson - Learning Rust with Game Development - YouTube](https://www.aliyundrive.com/s/AoLEhwsgv9P)|    
  
  

# 🏗 开源框架
  
## 值得新手关注的Rust项目

- [mini redis](https://github.com/tokio-rs/mini-redis) - 不完整的Redis客户端和服务器实现使用Tokio -仅为学习目的
- [async-graphql](https://github.com/sunli829/async-graphql) - 一个在Rust中实现的GraphQL服务器库
  
## 应用程序

- [alacritty](https://github.com/alacritty/alacritty) — 跨平台、GPU 增强的终端模拟器
- [AnderEnder/s3find-rs](https://github.com/AnderEnder/s3find-rs) — 用于遍历 Amazon S3 层次结构的命令行实用程序，类似于 Amazon S3 的 find
- [andschwa/rust-genetic-algorithm](https://github.com/andschwa/rust-genetic-algorithm) — 一种用于学术基准问题的遗传算法
- [asm-cli-rust](https://github.com/cch123/asm-cli-rust) — 一个用 Rust 编写的交互式程序集外壳.
- [ballista](https://github.com/ballista-compute/ballista) — 使用 Rust、Apache Arrow 和 Kubernetes 的分布式计算平台的 PoC！
- [cloudflare/boringtun](https://github.com/cloudflare/boringtun) — 用户空间 WireGuard VPN 实现
- [darrint/device-blocker](https://github.com/darrint/device-blocker) — 通过阻止家庭 Wifi 路由器上的互联网访问来限制儿童各种移动设备的屏幕时间.
- [denoland/deno](https://github.com/denoland/deno) — 使用 V8、Rust 和 Tokio 构建的安全 JavaScript/TypeScript 运行时
- [dlecan/generic-dns-update](https://github.com/dlecan/generic-dns-update) — 使用您的 IP 地址更新 DNS 区域文件的工具
- [Factotum](https://github.com/snowplow/factotum) — [A system to programmatically run data pipelines](https://snowplowanalytics.com/blog/2016/04/09/introducing-factotum-data-pipeline-runner/) 
- [fcsonline/drill](https://github.com/fcsonline/drill) — 受 Ansible 语法启发的 HTTP 负载测试应用程序
- [Fractalide](https://github.com/fractalide/fractalide) — 简单的 Rust 微服务
- [habitat](https://community.chef.io/tools/chef-habitat) — 一个工具 [Chef](https://www.chef.io/) 构建、部署和管理应用程序.
- [Herd](https://github.com/imjacobclark/Herd) — 一个实验性的 HTTP 负载测试应用程序
- [intecture/api](https://github.com/intecture/api) — API 驱动的服务器管理和配置工具
- [ivanceras/diwata](https://github.com/ivanceras/diwata) — postgresql 的数据库管理工具
- [jedisct1/flowgger](https://github.com/awslabs/flowgger) — 快速、简单和轻量级的数据收集器
- [kbknapp/docli](https://github.com/kbknapp/docli-rs) — 用于管理 DigitalOcean 基础设施的命令行实用程序 
- [kytan](https://github.com/changlan/kytan) — 高性能点对点 VPN
- [limonite](https://crates.io/crates/limonite) — 静态博客 / 网站生成器 
- [linkerd/linkerd2-proxy](https://github.com/linkerd/linkerd2-proxy) — Kubernetes 的超轻服务网格.
- [MaidSafe](https://maidsafe.net/) — 一个去中心化的平台.
- [mdBook](https://crates.io/crates/mdbook) — 从 Markdown 文件创建书籍的命令行实用程序 
- [nicohman/eidolon](https://github.com/nicohman/eidolon) — 适用于 linux 和 macosx 的无 Steam 和 drm 游戏注册表和启动器
- [notty](https://github.com/withoutboats/notty) — 一种新型终端
- [Pijul](https://pijul.org/) — 基于补丁的分布式版本控制系统
- [rsign](https://crates.io/crates/rsign) — 一个简单的命令行工具，用于生成 / 签署 / 验证旨在与 Minisign 兼容的数字签名 
- [Rudr](https://github.com/oam-dev/rudr) — Kubernetes 实现 [Open Application Model](https://oam.dev/) 规格
- [rx](https://github.com/cloudhead/rx) — 受 Vi 启发的现代像素艺术编辑器
- [Sandstorm Collections App](https://github.com/sandstorm-io/collections-app)
- [Servo](https://github.com/servo/servo) — 原型 Web 浏览器引擎
- [tiny](https://github.com/osa1/tiny) — 终端 IRC 客户端
- [trust-dns](https://crates.io/crates/trust-dns) — DNS 服务器
- [updns](https://github.com/wyhaya/updns) — DNS 代理工具
- [Weld](https://github.com/serayuzgur/weld) — 全假 REST API 生成器 
- [wezterm](https://github.com/wez/wezterm) — 一个gpu加速的跨平台终端模拟器和多路复用器
  
### 音频和音乐技术

- [enginesound](https://github.com/DasEtwas/enginesound) — 用于按程序生成半逼真引擎声音的 GUI 和命令行应用程序. 具有深度配置、可变采样率和频率分析窗口.
- [indiscipline/zrtstr](https://github.com/indiscipline/zrtstr) — 用于检查立体声 wav 文件是否为仿立体声（即具有相同通道）并将此类文件转换为单声道的命令行实用程序.
- [Lyriek](https://github.com/bartwillems/lyriek) — 一个多线程 GTK 3 应用程序，用于获取当前播放歌曲的歌词.
- [Phate6660/musinfo](https://github.com/Phate6660/musinfo) — 从 mpd 查询音乐信息并将其显示在通知中的程序.
- [Phate6660/rsmpc](https://github.com/Phate6660/rsmpc) — mpc 的实现，但不是直接实现，因为会有一些差异.
- [Phate6660/rsmpc](https://github.com/Phate6660/rsmpc-gui) — 用于 mpd 的 gtk 前端.
- [Polaris](https://github.com/agersant/polaris) — 音乐流媒体应用程序. 
- [Spotify TUI](https://github.com/Rigellute/spotify-tui) — 一个用 Rust 编写的用于终端的 Spotify 客户端. 
- [Spotifyd](https://github.com/Spotifyd/spotifyd) — 作为 UNIX 守护程序运行的开源 Spotify 客户端. 
  
### 加密数字货币

- [Bitcoin Satoshi's Vision](https://github.com/brentongunning/rust-sv) — 用于处理比特币 SV 的 Rust 库.
- [cardano-cli](https://github.com/input-output-hk/cardano-cli) — 卡尔达诺命令行界面 (CLI)
- [ChainX](https://github.com/chainx-org/ChainX) — Polkadot 上完全去中心化的链间加密资产管理.
- [CITA](https://github.com/citahub/cita) — 面向企业用户的高性能区块链内核.
- [coinbase-pro-rs](https://github.com/inv2004/coinbase-pro-rs) — Rust 中的 Coinbase pro 客户端，支持同步 / 异步 / websocket 
- [ethaddrgen](https://github.com/Limeth/ethaddrgen) — 用 Rust 制作的自定义以太坊虚地址生成器 
- [Grin](https://github.com/mimblewimble/grin/) — MimbleWimble 协议的演变
- [hdwallet](https://github.com/jjyr/hdwallet) — BIP-32 HD 钱包相关的密钥推导实用程序.
- [Holochain](https://github.com/holochain/holochain) — 区块链的可扩展 P2P 替代方案，适用于您一直想要构建的所有分布式应用程序. 旧仓库的链接是 [this](https://github.com/holochain/holochain-rust) 不再维护.[ibc-rs](https://github.com/informalsystems/ibc-rs) - Rust 的实现 [Interblockchain Communication](https://xn--ibc-3h3e109w.org/) 协议
- [infincia/bip39-rs](https://github.com/infincia/bip39-rs) — BIP39 的 Rust 实现.
- [Joystream](https://github.com/Joystream/joystream) — 一个用户管理的视频平台 
- [Diem](https://github.com/diem/diem) — Diem 的使命是建立一个简单的全球货币和金融基础设施，为数十亿人赋能.
- [Lighthouse](https://github.com/sigp/lighthouse) — Rust Ethereum 2.0 客户端
- [near/nearcore](https://github.com/near/nearcore) — 用于低端移动设备的去中心化智能合约平台.
- [Nervos CKB](https://github.com/nervosnetwork/ckb) — Nervos CKB 是一个公共的免许可区块链，是 Nervos 网络的公共知识层.
- [Nimiq](https://github.com/nimiq/core-rs) — Nimiq 节点的 Rust 实现
- [Parity-Bitcoin](https://github.com/paritytech/parity-bitcoin) — Parity 比特币客户端
- [Parity-Bridge](https://github.com/paritytech/parity-bridge) — 任何两个基于以太坊的网络之间的桥梁
- [Parity-Ethereum](https://github.com/openethereum/openethereum) — 快速、轻便、强大的以太坊客户端
- [Parity-Zcash](https://github.com/paritytech/parity-zcash) — Zcash 协议的 Rust 实现
- [Phala-Network/phala-blockchain](https://github.com/Phala-Network/phala-blockchain) — 基于 Intel SGX 和 Substrate 的机密智能合约区块链
- [Polkadot](https://github.com/paritytech/polkadot) — 具有集中安全性的异构多链技术
- [rbtc](https://github.com/lucawen/rbtc) — 将 BTC 转换为任何货币，反之亦然. 
- [rust-cardano](https://github.com/input-output-hk/rust-cardano) — Cardano 原语、助手和相关应用程序的 Rust 实现
- [Substrate](https://github.com/paritytech/substrate) — 用 Rust 编写的通用模块化区块链模板
- [tendermint-rs](https://github.com/informalsystems/tendermint-rs) - Tendermint 区块链数据结构和客户端的 Rust 实现
- [wagyu](https://github.com/AleoHQ/wagyu) [[wagyu](https://crates.io/crates/wagyu)] — 用于生成加密货币钱包的 Rust 库
- [zcash](https://github.com/zcash/zcash) — Zcash 是 “Zerocash” 协议的实现.
- [YeeCo yeeroot](https://github.com/yeeco/yeeroot) — YeeCo yeeroot 是一个无需许可、安全、高性能和可扩展的公共区块链平台，由基于 Rust 编写的 PoW 共识的全分片技术提供支持
  
### 数据库

- [indradb](https://crates.io/crates/indradb) — 基于 Rust 的图形数据库 
- [Materialize](https://github.com/MaterializeInc/materialize) - 由 Timely Dataflow 提供支持的流式 SQL 数据库：heavy_dollar_sign
- [noria](https://crates.io/crates/noria) — 用于 Web 应用程序后端的动态变化、部分状态的数据流
- [Lucid](https://github.com/lucid-kv/lucid) — High performance and distributed KV store accessible through a HTTP API.
- [ParityDB](https://github.com/paritytech/parity-db) — 快速可靠的数据库，针对读操作进行了优化
- [PumpkinDB](https://github.com/PumpkinDB/PumpkinDB) — 事件溯源数据库引擎 
- [seppo0010/rsedis](https://github.com/seppo0010/rsedis) — Rust 中的 Redis 重新实现 
- [Skytable](https://github.com/skytable/skytable) — 多模型 NoSQL 数据库 
- [tikv](https://github.com/tikv/tikv) — Rust 中的分布式 KV 数据库 
- [sled](https://crates.io/crates/sled) —（测试版）现代嵌入式数据库
- [TerminusDB](https://github.com/terminusdb/terminusdb-store) - 开源图形数据库和文档存储
  
### 模拟器

- [kondrak/rust64](https://github.com/kondrak/rust64) 
- [Ruffle](https://github.com/ruffle-rs/ruffle) — Ruffle 是用 Rust 编程语言编写的 Adobe Flash Player 模拟器. Ruffle 使用 WebAssembly 面向桌面和 Web.
- [Gekkio/mooneye-gb](https://github.com/Gekkio/mooneye-gb) 
- [mvdnes/rboy](https://github.com/mvdnes/rboy)
- [NivenT/RGB](https://github.com/nivent/RGB) 
- [mohanson/gameboy](https://github.com/mohanson/gameboy) — 全功能跨平台 GameBoy 模拟器. 永远的男孩！
- [michelhe/rustboyadvance-ng](https://github.com/michelhe/rustboyadvance-ng) - RustboyAdvance-ng 是一款 Gameboy Advance 模拟器，具有桌面、安卓和 [WebAssembly](https://michelhe.github.io/rustboyadvance-ng/) 支持.
- [iamsix/oxidenes](https://github.com/iamsix/oxidenes)
- [koute/pinky](https://github.com/koute/pinky) 
- [pcwalton/sprocketnes](https://github.com/pcwalton/sprocketnes)
- [Amjad50/plastic](https://github.com/Amjad50/plastic) — plastis 是一个用 Rust 构建的全功能 NES 模拟器.
- [rustation-ng](https://gitlab.com/flio/rustation-ng/) — 使用 Rust 的 Playstation 模拟器
- [pacmancoder/rustzx](https://github.com/pacmancoder/rustzx) 
- [rodrigorc/raze](https://github.com/rodrigorc/raze) — 对于 WebAssembly， [live version here](https://rodrigorc.github.io/raze/) * 虚拟男孩
- [emu-rs/rustual-boy](https://github.com/emu-rs/rustual-boy) 
- [mohanson/i8080](https://github.com/mohanson/i8080) — Rust 的 Intel 8080 cpu 模拟器 
  
### 游戏

- [lifthrasiir/angolmois-rust](https://github.com/lifthrasiir/angolmois-rust) — 一款支持 BMS 格式的极简音乐视频游戏
- [citybound](https://github.com/citybound/citybound) - 你应得的城市模拟
- [schulke-214/connect-four](https://github.com/schulke-214/connect-four) — 一个简单的连接四个实现.
- [doukutsu-rs](https://github.com/doukutsu-rs/doukutsu-rs) — 对 Cave Story 引擎的 Rust 重新实现，并进行了一些增强.
- [rsaarelm/magog](https://github.com/rsaarelm/magog) — Rust 中的 roguelike 游戏
- [schulke-214/rsnake](https://github.com/schulke-214/rsnake) — 用 Rust 编写的 Snake.
- [soydos](https://github.com/soydos/pusoy_dos2) — Pusoy Dos 的 wasm 实现
- [cristicbz/rust-doom](https://github.com/cristicbz/rust-doom) — Doom 的渲染器，可能会发展成为一款可玩的游戏 
- [Thinkofname/rust-quake](https://github.com/Thinkofname/rust-quake) — Rust 中的地震地图渲染器
- [rhex](https://github.com/dpc/rhex) — 六边形 ascii roguelike
- [garkimasera/rusted-ruins](https://github.com/garkimasera/rusted-ruins) - 具有像素艺术的可扩展开放世界流氓游戏
- [Veloren](https://gitlab.com/veloren/veloren) — 一个开放世界、开源的多人体素 RPG 游戏，目前处于 alpha 开发阶段
- [swatteau/sokoban-rs](https://github.com/swatteau/sokoban-rs) — 推箱子实现
- [aleshaleksey/TGWM](https://github.com/aleshaleksey/TGWM) — 具有回合制机制的 RPG（正在进行中）
- [ozkriff/zemeroth](https://github.com/ozkriff/zemeroth) — 一款小型 2D 回合制六角策略游戏
- [Zone of Control](https://github.com/ozkriff/zoc) — 回合制六角策略游戏 
- [phantomion/snake_game](https://github.com/phantomion/snake_game) - 用 Rust 编写的简单终端蛇游戏.

### 图形处理

- [Limeth/euclider](https://github.com/Limeth/euclider) — 实时 4D CPU 光线追踪器
- [RazrFalcon/resvg](https://github.com/RazrFalcon/resvg) — 一个 SVG 渲染库.
- [ivanceras/svgbob](https://github.com/ivanceras/svgbob) — 将 ASCII 图转换为 SVG 图形 
- [RazrFalcon/svgcleaner](https://github.com/RazrFalcon/svgcleaner) — 整理 SVG 图形
- [Twinklebear/tray_rust](https://github.com/Twinklebear/tray_rust) — 光线追踪器
- [turnage/valora](https://crates.io/crates/valora) — 生成美术图书馆 
- [mikigraf/Image-Processing-CLI-in-Rust](https://github.com/mikigraf/Image-Processing-CLI-in-Rust) — 用于处理图像、生成直方图的 CLI. 

### 工业自动化

- [locka99/opcua](https://github.com/locka99/opcua) —  [OPC UA](https://opcfoundation.org/about/opc-technologies/opc-ua/) 图书馆.
- [slowtec/tokio-modbus](https://github.com/slowtec/tokio-modbus) - 一种 [tokio](https://tokio.rs/)-based [modbus](https://modbus.org/) 图书馆. 
- [BiancoRoyal/modbus-iiot-rust](https://github.com/BiancoRoyal/modbus-iiot-rust) — 纯锈 [modbus](https://modbus.org/) 没有或更少依赖的库.
  
### 可观察性工具

- [timberio/vector](https://github.com/timberio/vector) — 高性能、日志、指标和事件路由器.
- [Mnwa/gtsa](https://github.com/Mnwa/gtsa) — 将 gelf 消息（Graylog 的消息）代理到 Sentry 的简单解决方案
- [OpenTelemetry](https://crates.io/crates/opentelemetry) — OpenTelemetry 提供一组 API、库、代理和收集器服务，以从您的应用程序中捕获分布式跟踪和指标. 您可以使用 Prometheus、Jaeger 和其他可观察性工具分析它们.

### 操作系统

- [nebulet/nebulet](https://github.com/nebulet/nebulet) — 实现在 Ring 0 中运行的 WebAssembly“用户模式” 的微内核.
- [redox-os/redox](https://gitlab.redox-os.org/redox-os/redox) 
- [thepowersgang/rust_os](https://github.com/thepowersgang/rust_os)
- [tock/tock](https://github.com/tock/tock) — 适用于基于 Cortex-M 的微控制器的安全嵌入式操作系统

### 生产能力

- [espanso](https://github.com/federico-terzi/espanso) — 一个用 Rust 编写的跨平台文本扩展器 [eureka](https://crates.io/crates/eureka) — 无需离开终端即可输入和存储您的想法的 CLI 工具
- [pier-cli/pier](https://github.com/pier-cli/pier) — 用于管理（添加、搜索元数据等）所有单行程序、脚本、工具和 CLI 的中央存储库
- [subilo](https://github.com/Bansco/subilo) - 持续部署代理

### 安全工具

- [kpcyrd/authoscope](https://github.com/kpcyrd/authoscope) — 一个可编写脚本的网络认证破解器
- [lethe](https://github.com/kostassoid/lethe) — 安全的跨平台驱动器擦除实用程序 
- [arvancloud/libinjection-rs](https://github.com/arvancloud/libinjection-rs) — Rust 绑定 [libinjection](https://github.com/client9/libinjection)
- [ripasso](https://github.com/cortex/ripasso/) — 密码管理器，与 pass 兼容的文件系统
- [kpcyrd/rshijack](https://github.com/kpcyrd/rshijack) — 一个 TCP 连接劫持者，对 shijack 进行 Rust 重写 
- [rustscan/rustscan](https://github.com/RustScan/RustScan) — 使用此端口扫描工具使 Nmap 更快
- [kpcyrd/sniffglue](https://github.com/kpcyrd/sniffglue) — 一个安全的多线程数据包嗅探器
- [kpcyrd/sn0int](https://github.com/kpcyrd/sn0int) — 半自动 OSINT 框架和包管理器   

### 系统工具

- [ajeetdsouza/zoxide](https://github.com/ajeetdsouza/zoxide/) — 一种快速替代 `cd` 的方法，可以学习你的习惯
- [bandwhich](https://github.com/imsnif/bandwhich) — 终端带宽利用工具
- [brocode/fblog](https://github.com/brocode/fblog) — 小型命令行 JSON 日志查看器 
- [buster/rrun](https://github.com/buster/rrun) — Linux 的命令启动器，类似于 gmrun
- [cristianoliveira/funzzy](https://github.com/cristianoliveira/funzzy) — 受启发的可配置文件系统观察器 [entr](http://eradman.com/entrproject/) 
- [dalance/procs](https://github.com/dalance/procs) — Rust 编写的 “ps” 的现代替代品
- [diskonaut](https://github.com/imsnif/diskonaut) — 终端可视化磁盘空间导航器
- [dust](https://github.com/bootandy/dust) — 更直观的 du 版本
- [ddh](https://github.com/darakian/ddh) — 快速重复文件查找器
- [fselect](https://crates.io/crates/fselect) — 使用类似 SQL 的查询查找文件 
- [gitui](https://github.com/extrawurst/gitui) - 用 Rust 编写的 git 快速终端客户端.
- [k0pernicus/zou](https://github.com/k0pernicus/zou) — 下载加速器
- [Kondo](https://github.com/tbillington/kondo) - 用于删除软件项目工件和回收磁盘空间的 CLI 和 GUI 工具
- [lotabout/rargs](https://github.com/lotabout/rargs) [[rargs](https://crates.io/crates/rargs)] — 支持模式匹配的 xargs + awk
- [lotabout/skim](https://github.com/lotabout/skim) — 纯锈的模糊取景器
- [mitnk/cicada](https://github.com/mitnk/cicada) — 一个类似 bash 的 Unix shell
- [mmstick/concurr](https://github.com/mmstick/concurr) — 带有客户端 - 服务器架构的 GNU Parallel 的替代方案
- [mmstick/fontfinder](https://github.com/mmstick/fontfinder) — 用于预览和安装 Google 字体的 GTK3 应用程序
- [mmstick/parallel](https://github.com/mmstick/parallel) — 重新实现 GNU Parallel
- [mmstick/tv-renamer](https://github.com/mmstick/tv-renamer) — 带有可选 GTK3 前端的电视剧重命名应用程序. 
- [nushell/nushell](https://github.com/nushell/nushell) — 一个新型Shell. 
- [organize-rt](https://gitlab.com/FixFromDarkness/organize-rt) — 根据正则表达式规则组织文件（默认为文件扩展名）.
- [orhun/kmon](https://github.com/orhun/kmon) — Linux 内核管理器和活动监视器 
- [Peltoche/lsd](https://github.com/Peltoche/lsd) — 一个 ls 有很多漂亮的颜色和很棒的图标 
- [ogham/exa](https://github.com/ogham/exa) — 'ls' 的替代品 
- [pop-os/debrep](https://github.com/pop-os/debrepbuild) — 用于构建和管理 APT 存储库的 APT 存储库工具
- [pop-os/popsicle](https://github.com/pop-os/popsicle) — GTK3 和 CLI 实用程序，用于并行刷新多个 USB 设备
- [pueue](https://github.com/nukesor/pueue) — 管理您长时间运行的 shell 命令.
- [Luminarys/synapse](https://github.com/Luminarys/synapse) — 灵活且快速的 BitTorrent 守护进程. 
- [pop-os/system76-power](https://github.com/pop-os/system76-power/) — 带有 CLI 工具的 Linux 电源管理守护进程（DBus 接口）.
- [mxseev/logram](https://github.com/mxseev/logram) — 将日志文件的更新推送到 Telegram
- [redox-os/ion](https://github.com/redox-os/ion) — 下一代系统外壳 
- [jamesbirtles/hotkey-rs](https://github.com/jamesbirtles/hotkey-rs) — 在 Rust 中收听全局热键的库
- [nivekuil/rip](https://github.com/nivekuil/rip) - 一种安全且符合人体工程学的替代`rm` 
- [sharkdp/bat](https://github.com/sharkdp/bat) — 有翅膀的 cat(1) 克隆体. 
- [sharkdp/fd](https://github.com/sharkdp/fd) — 一种简单、快速且用户友好的查找替代方案.
- [sitkevij/hex](https://github.com/sitkevij/hex) — 彩色的 hexdump 终端实用程序.
- [slai11/goto](https://github.com/slai11/goto) — 跳转到索引目录的简单且用户友好的方式.
- [m4b/bingrep](https://github.com/m4b/bingrep) — 通过来自各种操作系统和体系结构的二进制文件进行 Greps，并为它们着色. 
- [uutils/coreutils](https://github.com/uutils/coreutils) — GNU coreutils 的跨平台 Rust 重写
- [watchexec](https://github.com/watchexec/watchexec) — 执行命令以响应文件修改 
- [XAMPPRocky/tokei](https://github.com/XAMPPRocky/tokei) — 计算代码行数 
- [yake](https://crates.io/crates/yake) — Yake 是一个基于 yaml 文件的任务运行器
- [ytop](https://github.com/cjbassi/ytop) - 一个用 Rust 编写的 TUI 系统监视器 
- [cocom](https://github.com/LamdaLamdaLamda/cocom) - 纯粹用 Rust 编写的 NTP 客户端. 

### 文字编辑器

- [amp](https://amp.rs/) — 受 Vi/Vim 的启发. 
- [gchp/iota](https://github.com/gchp/iota) — 一个简单的文本编辑器
- [ilai-deutel/kibi](https://github.com/ilai-deutel/kibi) — 具有语法高亮、增量搜索等功能的小型 (≤1024 LOC) 文本编辑器.
- [vamolessa/pepper](https://github.com/vamolessa/pepper) [[pepper](https://crates.io/crates/pepper)] — 一个自以为是的模式编辑器，可简化从终端进行的代码编辑
- [mathall/rim](https://github.com/mathall/rim) — 用 Rust 编写的类似 Vim 的文本编辑器
- [ox](https://github.com/curlpipe/ox) — 在终端中运行的独立 Rust 文本编辑器！
- [Remacs](https://github.com/remacs/remacs) — 社区驱动的 Emacs 到 Rust 的移植.
- [xi-editor](https://github.com/xi-editor/xi-editor) — 一个现代编辑器，后端是用 Rust 编写的.
- [xray](https://github.com/atom-archive/xray) — 实验性的下一代基于电子的文本编辑器. 

### 文本处理

- [cpc](https://github.com/probablykasper/cpc) - 解析和计算数学字符串，支持单位和单位转换，从 “1+2” 到“1% 的回合（1 光年 / 14!s 到公里 / 小时）”.
- [grex](https://github.com/pemistahl/grex) — 用于从用户提供的测试用例生成正则表达式的命令行工具和库
- [dmerejkowsky/ruplacer](https://github.com/dmerejkowsky/ruplacer) — 在源文件中查找和替换文本
- [ripgrep](https://crates.io/crates/ripgrep) — 结合了 Silver Searcher 的可用性和 grep 的原始速度
- [phiresky/ripgrep-all](https://github.com/phiresky/ripgrep-all) — ripgrep，还可以搜索 PDF、电子书、Office 文档、zip、tar.gz 等.
- [replicadse/complate](https://github.com/replicadse/complate) — 一种终端内文本模板工具，用于标准化消息（如 GIT 提交）. 
- [sd](https://crates.io/crates/sd) — 直观的查找和替换 CLI
- [lavifb/todo_r](https://github.com/lavifb/todo_r) — 用一个命令查找所有 TODO 笔记！ 
- [whitfin/runiq](https://github.com/whitfin/runiq) — 从未排序的输入中过滤重复行的有效方法.
- [whitfin/bytelines](https://github.com/whitfin/bytelines) — 将输入行读取为字节片以提高效率.
- [vishaltelangre/ff](https://github.com/vishaltelangre/ff) — 按名称查找文件 (ff)！ 
- [xsv](https://crates.io/crates/xsv) — 一个快速的 CSV 命令行工具（切片、索引、选择、搜索、采样等）
- [Lisprez/so_stupid_search](https://github.com/Lisprez/so_stupid_search) — 一个简单快速的人类字符串搜索工具

### 图像处理

- [Imager](https://github.com/imager-io/imager) — 自动图像优化.

### 实用工具

- [aleshaleksey/AZDice](https://github.com/aleshaleksey/AZDice) — 桌面家庭酿酒商的骰子成功分发生成器. 
- [yaa110/cb](https://github.com/yaa110/cb) — 管理剪贴板的命令行界面 
- [brycx/checkpwn](https://github.com/brycx/checkpwn) — 一个 Have I Being Pwned (HIBP) 命令行实用工具，可让您轻松检查被盗用的帐户和密码.
- [vamolessa/copycat](https://github.com/vamolessa/copycat) [[copycat](https://crates.io/crates/copycat)] — 一个简单的剪贴板 cli 界面，适用于具有文本和 bmp 支持的窗口
- [evansmurithi/cloak](https://github.com/evansmurithi/cloak) — 命令行 OTP（一次性密码）身份验证器应用程序. 
- [replydev/cotp](https://github.com/replydev/cotp) - 与外部备份兼容的值得信赖的加密一次性密码验证器应用程序. 
- [rustdesk/rustdesk](https://github.com/rustdesk/rustdesk) - 远程桌面应用程序. 
- [arthrp/consoletimer](https://github.com/arthrp/consoleTimer) — 终端的简单计时器.
- [tversteeg/emplace](https://github.com/tversteeg/emplace) — 在多台机器上同步已安装的包
- [unrelentingtech/freepass](https://github.com/unrelentingtech/freepass) — 高级用户的免费密码管理器.
- [yoannfleurydev/gitweb](https://github.com/yoannfleurydev/gitweb) — 在浏览器中打开当前远程存储库.
- [mme](https://github.com/GoberInfinity/mme) — 命令行工具来记住您有时忘记的命令. 
- [raftario/licensor](https://github.com/raftario/licensor) — 将许可证写入标准输出
- [arthrp/quick-skeleton](https://github.com/arthrp/quick-skeleton) — 项目脚手架工具，类似于 Yeoman 和 Slush. 
- [repoch](https://github.com/lucawen/repoch) — 将纪元转换为日期时间，将日期时间转换为纪元 
- [whitfin/s3-concat](https://github.com/whitfin/s3-concat) — 使用灵活模式远程连接 Amazon S3 文件的命令行工具.
- [whitfin/s3-meta](https://github.com/whitfin/s3-meta) — 用于收集有关 Amazon S3 存储桶的元数据的命令行工具.
- [whitfin/s3-utils](https://github.com/whitfin/s3-utils) — 一个包含基于 Amazon S3 的实用程序的小工具，可提供额外的便利 API.
- [gorros/s3-edit-rs](https://github.com/gorros/s3-edit-rs) — 直接在 Amazon S3 上编辑文件的命令行工具.
- [fcsonline/tmux-thumbs](https://github.com/fcsonline/tmux-thumbs) — 用 Rust 编写的 tmux-finger 的闪电般快速版本，像 vimium/vimperator 一样复制 / 粘贴 tmux.
- [amar-laksh/workstation](https://github.com/amar-laksh/workstation) — 一个命令行工具，可帮助您管理工作站，让您远离屏幕、在您不在时锁定屏幕以及使用 OPENCV 进行其他操作！
- [guoxbin/dtool](https://github.com/guoxbin/dtool) — 一个有用的命令行工具集合，用于协助开发，包括转换、编解码器、散列、加密等.
- [nomino](https://github.com/yaa110/nomino) — 开发人员批量重命名实用程序 
- [barberousse](https://github.com/zeapo/barberousse) — AWS Secrets Manager 编辑器 
- [vamolessa/verco](https://github.com/vamolessa/verco) [[verco](https://crates.io/crates/verco)] — 一个简单的 Git/Hg tui 客户端，专注于键盘快捷键
  
### 视频

- [Phate6660/rsmpv](https://github.com/Phate6660/rsmpv) — MPV 控制器，需要在 MPV 中启用 IPC.
- [tgotwig/vidmerger](https://github.com/tgotwig/vidmerger) — ffmpeg 的包装器，可简化多个视频的合并
- [xiph/rav1e](https://github.com/xiph/rav1e) — 最快、最安全的 AV1 编码器.
- [yuvadm/slingr](https://github.com/yuvadm/slingr) — 一个简单的 CLI，用于通过本地网络将媒体文件流式传输到 UPnP 媒体渲染器
- [yuvadm/streamlib](https://github.com/streamlib/streamlib) — 从命令行播放您最喜欢的实时视频和音频流

### 虚拟化技术

- [firecracker-microvm/firecracker](https://github.com/firecracker-microvm/firecracker) — 用于容器工作负载的轻量级虚拟机 [Firecracker Microvm](https://firecracker-microvm.github.io/)
- [oracle/railcar](https://github.com/oracle/railcar) — Rust 中类似 Docker 的容器 OCI 运行时实现
- [tailhook/vagga](https://github.com/tailhook/vagga) — 一个没有守护进程的容器化工具

### Web

- [Plume-org/Plume](https://github.com/Plume-org/Plume) — ActivityPub 联合博客应用程序
- [LemmyNet/lemmy](https://github.com/LemmyNet/lemmy) — 联邦宇宙的链接聚合器 / reddit 克隆

### Web Servers

- [mufeedvh/binserve](https://github.com/mufeedvh/binserve) — 极快的静态 Web 服务器，在单个二进制文件中具有路由、模板和安全性，您可以使用零代码进行设置 
- [thecoshman/http](https://github.com/thecoshman/http) — 请托管这些东西 — 一个基本的 http 服务器，用于快速简单地托管文件夹 
- [svenstaro/miniserve](https://github.com/svenstaro/miniserve) — 一个小型的、自包含的跨平台 CLI 工具，允许您只获取二进制文件并通过 HTTP 提供一些文件
- [TheWaWaR/simple-http-server](https://github.com/TheWaWaR/simple-http-server) — 简单的静态 http 服务器
- [wyhaya/see](https://github.com/wyhaya/see) — 静态 HTTP 文件服务器
- [ronanyeah/rust-hasura](https://github.com/ronanyeah/rust-hasura) — Rust GraphQL 服务器如何用作远程模式的演示 [Hasura](https://hasura.io/) 
  
## 开发工具
  
- [clippy](https://crates.io/crates/clippy)
- [clog-tool/clog-cli](https://github.com/clog-tool/clog-cli) — 从 git 元数据生成变更日志 ([conventional changelog](https://blog.thoughtram.io/announcements/tools/2014/09/18/announcing-clog-a-conventional-changelog-generator-for-the-rest-of-us.html)) 
- [dan-t/rusty-tags](https://github.com/dan-t/rusty-tags) — 为货物项目及其所有依赖项创建 ctags/etags 
- [datanymizer/datanymizer](https://github.com/datanymizer/datanymizer) - 强大的数据库匿名器，具有灵活的规则
- [delta](https://crates.io/crates/git-delta) — git 和 diff 输出的语法高亮器
- [dotenv-linter](https://github.com/dotenv-linter/dotenv-linter) — 用于 `.env` 文件的 Linter[frewsxcv/crate-deps](https://github.com/frewsxcv/crate-deps) — 为 crates.io 上托管的 crate 生成依赖图的图像
- [geiger](https://github.com/rust-secure-code/cargo-geiger) — 一个程序，列出与在 Rust crate 及其所有依赖项中使用不安全 Rust 代码相关的统计信息m/cargo-geiger/cargo-geiger/_build/latest?definitionId=1&branchName=master)
- [git-journal](https://github.com/saschagrunert/git-journal/) — Git 提交消息和变更日志生成框架 
- [gstats](https://github.com/boonshift/gstats/) — 用于打印当前目录下所有 git 存储库的开发人员方便摘要的命令行工具
- [rust-lang/rustfix](https://github.com/rust-lang/rustfix) — 自动应用 rustc 提出的建议
- [just](https://github.com/casey/just) — 用于特定项目任务的便捷命令运行器
- [mask](https://github.com/jakedeichert/mask) — 由一个简单的 Markdown 文件定义的 CLI 任务运行器
- [Module Linker](https://github.com/fiatjaf/module-linker) —在 GitHub 的 `mod`、`use` 和 `extern crate` 语句中添加 `<a>` 链接到引用的扩展.
- [ptags](https://github.com/dalance/ptags) — git 存储库的并行通用 ctags 包装器 
- [Racer](https://github.com/racer-rust/racer) — Rust 的代码完成 
- [rustfmt](https://github.com/rust-lang/rustfmt) — Rust 代码格式化程序
- [Rustup](https://github.com/rust-lang/rustup) — Rust 工具链安装程序 
- [Rust Language Server](https://github.com/rust-lang/rls) — 在后台运行的服务器，为 IDE、编辑器和其他工具提供有关 Rust 程序的信息
- [Rust Regex Playground](https://2fd.github.io/rust-regex-playground/#method=find&regex=\w%2B&text=abc) — 评估 Rust 正则表达式的 Web 工具
- [Rust Search Extension](https://github.com/huhu/rust-search-extension) — 一个方便的浏览器扩展，用于在地址栏（多功能框）中搜索 crate 和文档. 
- [artifact](https://github.com/vitiral/artifact) — 为开发人员制作的设计文档工具 
- [semantic-rs](https://github.com/semantic-rs/semantic-rs) — 自动 crate 发布
- [fw](https://github.com/brocode/fw) — 工作空间生产力助推器 
- [tinyrick](https://github.com/mcandre/tinyrick) 一个基本的任务依赖工具，强调 Rust 功能而不是原始 shell 命令.
- [scriptisto](https://github.com/igor-petruk/scriptisto) 一种与语言无关的 “shebang 解释器”，它使您能够用编译语言编写一个文件脚本.
 
### 系统编译

- [Cargo](https://crates.io/) — Rust 包管理器
- [cargo-benchcmp](https://crates.io/crates/cargo-benchcmp) — 比较 Rust 微基准的实用程序 
- [cargo-bitbake](https://crates.io/crates/cargo-bitbake) — 一个货物扩展，可以利用 meta-rust 中的类生成 BitBake 配方
- [cargo-cache](https://crates.io/crates/cargo-cache) - 检查 / 管理 / 清理你的货物缓存（`~/.cargo/`/`${CARGO_HOME}`），打印尺寸等
- [cargo-check](https://crates.io/crates/cargo-check) — `cargo rustc -- -Zno-trans` 的包装器，如果您只需要正确性检查，它可以帮助运行更快的编译
- [cargo-count](https://crates.io/crates/cargo-count) — 列出有关货物项目的源代码计数和详细信息，包括不安全统计数据
- [cargo-deb](https://crates.io/crates/cargo-deb) — 生成二进制 Debian 软件包
- [cargo-deps](https://crates.io/crates/cargo-deps) — 构建 Rust 项目的依赖图
- [cargo-do](https://crates.io/crates/cargo-do) — 连续运行多个货物命令 
- [cargo-ebuild](https://crates.io/crates/cargo-ebuild) — 可以使用树内 eclasses 生成 ebuild 的货物扩展
- [cargo-edit](https://crates.io/crates/cargo-edit) — 允许您通过从命令行读取 / 写入 Cargo.toml 文件来添加和列出依赖项
- [cargo-generate](https://github.com/cargo-generate/cargo-generate) 通过利用预先存在的 git 存储库作为模板来生成 Rust 项目.
- [cargo-get](https://crates.io/crates/cargo-get) - Cargo 插件可以轻松地从 Cargo.toml 文件中查询信息 
- [cargo-graph](https://crates.io/crates/cargo-graph) — 更新了具有附加功能的 `cargo-dot` 分支. 未维护，请参阅`cargo-deps` 
- [cargo-info](https://crates.io/crates/cargo-info) — 从命令行查询 crates.io 以获取 crates 详细信息 
- [cargo-license](https://crates.io/crates/cargo-license) — 一个货物子命令，用于快速查看所有依赖项的许可证.
- [cargo-make](https://crates.io/crates/cargo-make) — Rust 任务运行器和构建工具. 
- [cargo-modules](https://crates.io/crates/cargo-modules) — 一个货物插件，用于显示板条箱模块的树状概览. 
- [cargo-multi](https://crates.io/crates/cargo-multi) — 在多个板条箱上运行指定的货物命令
- [cargo-outdated](https://crates.io/crates/cargo-outdated) — 在新版本的 Rust 依赖项可用或过时时显示
- [cargo-release](https://crates.io/crates/cargo-release) — 用于发布 git 管理的货物项目、构建、标记、发布、文档和推送的工具 
- [cargo-script](https://crates.io/crates/cargo-script) — 让人们快速、轻松地运行 Rust “脚本”，它可以利用 Cargo 的包生态系统
- [cargo-testify](https://crates.io/crates/cargo-testify) — 监视文件更改、运行测试并通过友好的操作系统通知通知结果
- [cargo-tree](https://github.com/sfackler/cargo-tree) – Cargo 子命令，以树状格式可视化 crate 的依赖关系图
- [cargo-update](https://crates.io/crates/cargo-update) — 用于检查和应用更新已安装的可执行文件的货物子命令 
- [cargo-watch](https://crates.io/crates/cargo-watch) — 货物在源更改时编译项目的实用程序
- [liuchong/cargo-x](https://github.com/liuchong/cargo-x) ——一个非常简单的第三方 cargo 子命令来执行自定义命令
- [dtolnay/cargo-expand](https://github.com/dtolnay/cargo-expand) — 扩展源代码中的宏
- [Devolutions/CMakeRust](https://github.com/Devolutions/CMakeRust) — 用于将 Rust 库集成到 CMake 项目中
- [SiegeLord/RustCMake](https://github.com/SiegeLord/RustCMake) — 一个示例项目，展示了 CMake 与 Rust 的使用 
- [icepuma/rust-action](https://github.com/icepuma/rust-action) ——Rust github 动作
- [peaceiris/actions-mdbook](https://github.com/peaceiris/actions-mdbook) — mdBook 的 GitHub 操作
- GitHub 网络钩子
- [snare](https://tratt.net/laurie/src/snare/) — GitHub webhooks 运行器守护进程
- 网络包
- [mxseev/rust-loader](https://github.com/mxseev/rust-loader) — Webpack Rust 加载器 (wasm)

### 调试

- [rust-gdb](https://github.com/rust-lang/rust/blob/master/src/etc/rust-gdb)
- [gdbgui](https://github.com/cs01/gdbgui) — 基于浏览器的 gdb 前端，用于调试 C、C++、Rust 和 Go.
- [lldb_batchmode.py](https://github.com/rust-lang/rust/blob/master/src/etc/lldb_batchmode.py) — 允许以类似于 GDB 的批处理模式的方式使用 LLDB.
- [CodeLLDB](https://marketplace.visualstudio.com/items?itemName=vadimcn.vscode-lldb) — 一个 LLDB 扩展 [Visual Studio Code](https://code.visualstudio.com/).

### 部署

- [emk/rust-musl-builder](https://github.com/emk/rust-musl-builder) — 用于使用 musl-libc 和 musl-gcc 编译静态 Rust 二进制文件的 Docker 映像，以及有用的 C 库的静态版本
- [kpcyrd/mini-docker-rust](https://github.com/kpcyrd/mini-docker-rust) — 一个非常小的 Rust docker 镜像的示例项目 
- [liuchong/docker-rustup](https://github.com/liuchong/docker-rustup) — 多版本（使用 musl 工具）Rust Docker 镜像
- [messense/rust-musl-cross](https://github.com/messense/rust-musl-cross) — 使用 musl-cross 编译静态 Rust 二进制文件的 Docker 镜像 
- [rust-lang-nursery/docker-rust](https://github.com/rust-lang/docker-rust) — 官方 Rust Docker 镜像
- [wasm-template-rust](https://github.com/sn99/wasm-template-rust) — Rust 发布到 gh-pages 的 wasm 模板，无需 npm-deploy 
- [DenisKolodin/rust-app-engine](https://github.com/DenisKolodin/rust-app-engine) — App Engine Rust 样板
- [emk/heroku-buildpack-rust](https://github.com/emk/heroku-buildpack-rust) — Heroku 上的 Rust 应用程序构建包

### 嵌入式

- [japaric/rust-cross](https://github.com/japaric/rust-cross) ——关于交叉编译 Rust 程序你需要知道的一切
- [japaric/xargo](https://github.com/japaric/xargo) — 轻松地将 Rust 程序交叉编译到自定义的裸机目标，如 ARM Cortex-M
- [Ogeon/rust-on-raspberry-pi](https://github.com/Ogeon/rust-on-raspberry-pi) — 有关如何为 Raspberry Pi 交叉编译 Rust 项目的说明. * 阿杜诺
- [avr-rust/ruduino](https://github.com/avr-rust/ruduino) `t Arduino Uno 的可重用组件.

### FFI

也可以看看 [Foreign Function Interface](https://doc.rust-lang.org/book/first-edition/ffi.html), [The Rust FFI Omnibus](http://jakegoulding.com/rust-ffi-omnibus/) （使用其他语言用 Rust 编写的代码的示例集合）和 [FFI examples written in Rust](https://github.com/alexcrichton/rust-ffi-examples).

- [rlhunt/cbindgen](https://github.com/eqrion/cbindgen) — 从 Rust 源文件生成 C 头文件. 在 Gecko 中用于 WebRender 
- [Sean1708/rusty-cheddar](https://github.com/Sean1708/rusty-cheddar) — 从 Rust 源文件生成 C 头文件
- [rust-lang/rust-bindgen](https://github.com/rust-lang/rust-bindgen) — Rust 绑定生成器
- [dtolnay/cxx](https://github.com/dtolnay/cxx) — Rust 和 C++ 之间的安全互操作
- [rust-cpp](https://crates.io/crates/cpp) - 直接在 Rust 中嵌入 C++ 代码
- [rusterlium/rustler](https://github.com/rusterlium/rustler) — 用于创建 Erlang NIF 函数的安全 Rust 桥 
- [mgattozzi/curryrs](https://github.com/mgattozzi/curryrs) — 弥合 Haskell 和 Rust 之间的差距
- [mgattozzi/haskellrs](https://github.com/mgattozzi/haskellrs) — Haskell FFI 示例中的 Rust
- [mgattozzi/rushs](https://github.com/mgattozzi/rushs) — Rust FFI 示例中的 Haskell
- [j4rs](https://crates.io/crates/j4rs) — 使用 Rust 中的 Java 
- [bennettanderson/rjni](https://github.com/benanders/rjni) — 使用 Rust 中的 Java
- [drrb/java-rust-example](https://github.com/drrb/java-rust-example) — 使用 Java 中的 Rust
- [jni](https://crates.io/crates/jni) — 使用 Java 中的 Rust
- [jni-sys](https://crates.io/crates/jni-sys) — 对应于 jni.h 的 Rust 定义 
- [rucaja](https://crates.io/crates/rucaja) — 使用 Rust 中的 Java 
- [rawrafox/rust-jdbc](https://github.com/rawrafox/rust-jdbc) — 使用来自 Rust 的 JDBC
- [jcmoyer/rust-lua53](https://github.com/jcmoyer/rust-lua53) — 用于 Rust 的 Lua 5.3 绑定
- [lilyball/rust-lua](https://github.com/lilyball/rust-lua) — Safe Rust bindings to Lua 5.1
- [tickbh/td_rlua](https://github.com/tickbh/td_rlua) — Rust 的零成本高级 lua 5.3 包装器
- [tomaka/hlua](https://github.com/tomaka/hlua) - 与 Lua 交互的 Rust 库 
- [anima-engine/mrusty](https://github.com/anima-engine/mrusty) — Rust 的 mruby 安全绑定
- [neon-bindings/neon](https://github.com/neon-bindings/neon) — Rust 绑定，用于编写安全且快速的原生 Node.js 模块
- [infinyon/node-bindgen](https://github.com/infinyon/node-bindgen) - 使用 Rust 生成 nodejs 模块的简单方法 * 目标 - C
- [SSheldon/rust-objc](https://github.com/SSheldon/rust-objc) — Rust 的 Objective-C 运行时绑定和包装器
- [vickenty/mi-rust](https://github.com/vickenty/mi-rust) — 添加对 M::I 的支持，以使用 Cargo 构建模块
- [vickenty/perl-xs](https://github.com/vickenty/perl-xs) — 使用 Rust 创建 Perl XS 模块 
- [getsentry/milksnake](https://github.com/getsentry/milksnake) — python setuptools 的扩展，它允许您以可想象的最便携的方式在 Python 轮子中分发动态链接库.
- [dgrunwald/rust-cpython](https://github.com/dgrunwald/rust-cpython) — Python 绑定
- [PyO3/PyO3](https://github.com/PyO3/PyO3) — Python 解释器的 Rust 绑定 
- [d-unseductable/ruru](https://github.com/d-unseductable/ruru) — 用 Rust 编写的原生 Ruby 扩展 
- [danielpclark/rutie](https://github.com/danielpclark/rutie) — 用 Rust 编写的原生 Ruby 扩展，反之亦然 
- [tildeio/helix](https://github.com/tildeio/helix) — 用 Rust 编写 Ruby 类 
- [rustwasm/wasm-pack](https://github.com/rustwasm/wasm-pack) —   打包 wasm 并发布到 npm！
- [rustwasm/wasm-bindgen](https://github.com/rustwasm/wasm-bindgen) — 一个促进 wasm 模块和 JS 之间高级交互的项目. 
- [rhysd/wain](https://github.com/rhysd/wain) - wain：在 Safe Rust 中从零开始的 WebAssembly 解释器，零依赖 
  
### IDEs

也可以看看 [Are we (I)DE yet?](https://areweideyet.com/) 和 [Rust Tools](https://www.rust-lang.org/tools).

- Atom

  - [zargony/atom-language-rust](https://github.com/zargony/atom-language-rust)
  - [rust-lang/atom-ide-rust](https://github.com/rust-lang/atom-ide-rust) — Rust IDE 对 Atom 的支持，由 Rust 语言服务器 (RLS) 提供支持

- Eclipse

  - [Eclipse Corrosion](https://github.com/eclipse/corrosion)
  - [RustDT](https://github.com/RustDT/RustDT) 

- Emacs

  - [rust-mode](https://github.com/rust-lang/rust-mode) — Rust 主要模式
  - [rustic](https://github.com/brotzeit/rustic) - Emacs 的 Rust 开发环境 
  - [flycheck-rust](https://github.com/flycheck/flycheck-rust) — Rust 支持 [Flycheck](https://github.com/flycheck/flycheck)
  - [emacs-racer](https://github.com/racer-rust/emacs-racer) — 自动完成（另见 [company](https://company-mode.github.io/) 和 [auto-complete](https://github.com/auto-complete/auto-complete))

- [gitpod.io](https://gitpod.io/) — 基于 Rust 语言服务器的具有完整 Rust 支持的在线 IDE

- [gnome-builder](https://wiki.gnome.org/Apps/Builder) 自版本 3.22.2 起原生支持 Rust 和 Cargo

- Kakoune

  - [kak-lsp/kak-lsp](https://github.com/kak-lsp/kak-lsp/) — [LSP](https://microsoft.github.io/language-server-protocol/) 客户. 在 Rust 中实现并支持 rls 开箱即用.

- NetBeans

  - [drrb/rust-netbeans](https://github.com/drrb/rust-netbeans)

- IntelliJ

  - [intellij-rust/intellij-rust](https://github.com/intellij-rust/intellij-rust) 
  - [intellij-rust/intellij-toml](https://github.com/intellij-rust/intellij-toml) — 基本的 Toml 支持

- [Ride](https://github.com/madeso/ride)

- [SolidOak](https://github.com/oakes/SolidOak) — 一个简单的 Rust IDE，基于 GTK+ 和 [Neovim](https://github.com/neovim/neovim)

- Sublime Text

  - [rust-lang/rust-enhanced](https://github.com/rust-lang/rust-enhanced) — 官方 Rust 包
  - [sublimehq/packages](https://github.com/sublimehq/Packages/tree/master/Rust) — 原生 Sublime 支持（已安装）

- Vim

  — 无处不在的文本编辑器

  - [rust.vim](https://github.com/rust-lang/rust.vim) — 提供文件检测、语法高亮、格式化、Syntastic 集成等.
  - [vim-cargo](https://github.com/timonv/vim-cargo) — 命令绑定以从 vim 快速运行货物.
  - [vim-racer](https://github.com/racer-rust/vim-racer) — 允许 vim 使用 [Racer](https://github.com/racer-rust/racer) 用于 Rust 代码完成和导航.
  - [autozimu/LanguageClient-neovim](https://github.com/autozimu/LanguageClient-neovim) — [LSP](https://microsoft.github.io/language-server-protocol/) 客户. 在 Rust 中实现并支持 rls 开箱即用

- 视觉工作室

  - [PistonDevelopers/VisualRust](https://github.com/PistonDevelopers/VisualRust) — Rust 的 Visual Studio 扩展
  - [dgriffen/rls-vs2017](https://github.com/ZoeyR/rls-vs2017) — 对 Visual Studio 2017 预览版的 Rust 支持

- Visual Studio Code

  - [rust-lang/rls-vscode](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust) — 对 Visual Studio Code 的 Rust 支持
  - [rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer) — RLS 的替代 Rust 语言服务器
  - [CodeLLDB](https://marketplace.visualstudio.com/items?itemName=vadimcn.vscode-lldb) — 一个 LLDB 扩展
  - [crates](https://github.com/serayuzgur/crates) — crates 是 crates.io 依赖项的扩展. 
  
### 图像识别

- [sfikas/rusteval](https://github.com/sfikas/rusteval) — 用于评估检索算法输出的工具 

### 分析

- [bheisler/criterion.rs](https://github.com/bheisler/criterion.rs) — 统计驱动的 Rust 基准测试库
- [sharkdp/hyperfine](https://github.com/sharkdp/hyperfine) — 命令行基准测试工具 
- [performancecopilot/hornet](https://github.com/performancecopilot/hornet) — Performance Co-Pilot 内存映射值检测库 
- [koute/memory-profiler](https://github.com/koute/memory-profiler) — Linux 的内存分析器 
- [ellisonch/rust-stopwatch](https://github.com/ellisonch/rust-stopwatch) — 一个秒表库 
- [mrhooray/torch](https://github.com/mrhooray/torch) — 根据 DWARF 调试信息生成 FlameGraphs
- [llogiq/flame](https://github.com/llogiq/flame) 

### Services

- [deps.rs](https://github.com/deps-rs/deps.rs) — 检测过时或不安全的依赖项
- [docs.rs](https://docs.rs/) — 自动生成 crate 文档
  
### 静态分析

- [facebookexperimental/MIRAI](https://github.com/facebookexperimental/mirai) — 一个在 Rust 的中级中间表示 (MIR) 上运行的抽象解释器
- [static_assertions](https://crates.io/crates/static_assertions) — 编译时断言以确保满足不变量 

### 测试

- [laboratory](https://crates.io/crates/laboratory) — 一个简单、富有表现力的 Rust 单元测试框架 
- [cucumber-rust](https://crates.io/crates/cucumber-rust) — Rust 的 Cucumber 测试框架的实现.
- [demonstrate](https://crates.io/crates/demonstrate) — 声明式测试框架 
- [httpmock](https://github.com/alexliesenfeld/httpmock) — HTTP 模拟 
- [mockiato](https://crates.io/crates/mockiato) — 一个严格但友好的 Rust 2018 模拟库
- [mutagen](https://crates.io/crates/mutagen) — 一个源级变异测试框架（仅限每晚）
- [AlKass/polish](https://github.com/AlKass/polish) — 迷你测试 / 测试驱动框架 
- [proptest](https://crates.io/crates/proptest) — 受启发的属性测试框架 [Hypothesis](https://hypothesis.works/) Python 框架
- [quickcheck](https://crates.io/crates/quickcheck) — 一个 Rust 实现 [QuickCheck](https://wiki.haskell.org/Introduction_to_QuickCheck1) 
- [mockito](https://crates.io/crates/mockito) — HTTP 模拟 
- [speculate](https://crates.io/crates/speculate) — 一个 RSpec 启发了 Rust 的最小测试框架
- [rstest](https://crates.io/crates/rstest) — Rust 的基于夹具的测试框架
- [ruspec](https://crates.io/crates/ruspec) — 像 Rspec 测试框架一样用 Rust 编写 
- [rust-fuzz/afl.rs](https://github.com/rust-fuzz/afl.rs) — 一个 Rust 模糊器，使用 [AFL](https://lcamtuf.coredump.cx/afl/) 
- [tarpaulin](https://crates.io/crates/cargo-tarpaulin) — 为 Rust 设计的代码覆盖率工具 
- [trust](https://github.com/japaric/trust) — Travis CI 和 AppVeyor 模板，用于在 5 种架构上测试您的 Rust crate 并发布其适用于 Linux、macOS 和 Windows 的二进制版本
- [fake-rs](https://github.com/cksac/fake-rs) — 生成假数据的库 
- [goldenfile](https://github.com/calder/rust-goldenfile) - 一个为 Goldenfile 测试提供简单 API 的库.
- [cargo-dinghy](https://crates.io/crates/cargo-dinghy/) - 简化在智能手机和其他小型处理器设备上运行库测试和工作台的货物扩展.

### 翻译器

- [immunant/c2rust](https://github.com/immunant/c2rust) — 在 Clang/LLVM 之上构建的 C 到 Rust 翻译器和交叉检查器. 
- [jameysharp/corrode](https://github.com/jameysharp/corrode) — 用 Haskell 编写的 AC 到 Rust 翻译器.

## 收集系统信息

- [Phate6660/nixinfo](https://github.com/Phate6660/nixinfo) [[crate](https://crates.io/crates/nixinfo)] — 一个用于收集系统信息（如 CPU、发行版、环境、内核等）的 lib crate.
  
# 🐂 大牛语录
  
### Matthieum:
  
“Rust 使编写正确且可读的代码变得更容易，同时获得两者并非巧合。

所有权/借用机制（对生命周期、别名和可变性的严格控制）在生成的软件的数据流中强制执行某种简单性，您可以在其他编程语言中获得这种简单性，但通常不会，因为该语言更宽松你得到了一个更复杂的流程。

你是否曾经在 Java 中调试过 ConcurrentModificationException？当您修改正在迭代的容器时会发生这种情况。当您有一系列回调/观察者时，意外地有导致此异常的循环引用非常容易。在 Rust 中，要解决这种情况，你必须使用 RefCell 或等价物，它应该让您停下来。”


## 联系专栏

#### 关注微信公众号【后台服务架构师】——【联系我们】，获取本repo最全PDF学习文档！

<img width="65%" height="65%" src="https://user-images.githubusercontent.com/87457873/130796999-03af3f54-3719-47b4-8e41-2e762ab1c68b.png"/>
  
  
  
  
  
