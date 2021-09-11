# 🏄💨【最安全的编程语言】Rust工程师枕边资料，大牛文章，开源框架，官方文档，视频，推荐书籍，学习干货，大牛语录

<div align=center>

![rust](https://user-images.githubusercontent.com/87457873/132184451-55f1125e-acad-4cc7-9e56-ecbffc0db412.png)
  
## 一个安全、并发、实用的系统语言

<br>
<br>
  
   [🏝<br>&nbsp;&nbsp;&nbsp; &nbsp;环境搭建&nbsp;&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E7%8E%AF%E5%A2%83%E6%90%AD%E5%BB%BA)  |[📕<br>&nbsp;&nbsp;&nbsp; 入门秘笈&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88-pdf%E6%A1%A3%E4%B8%8B%E8%BD%BD)|  [📖<br>&nbsp;&nbsp;&nbsp; 推荐书籍&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E6%8E%A8%E8%8D%90%E4%B9%A6%E7%B1%8D)
:-------: | :-------: | :---------:
 **[📑<br>精选文章](https://github.com/0voice/Understanding_in_Rust#-%E5%A4%A7%E7%89%9B%E6%96%87%E7%AB%A0)**  |  **[📰<br>官方文档](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E5%AE%98%E6%96%B9%E6%96%87%E6%A1%A3)**|  **[✈<br> 杂货铺](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E6%9D%82%E8%B4%A7%E9%93%BA)**
**[💽<br>视频](https://github.com/0voice/Understanding_in_Rust#-%E8%A7%86%E9%A2%91)** | **[🏗<br>开源框架](https://github.com/0voice/Understanding_in_Rust#-%E5%BC%80%E6%BA%90%E6%A1%86%E6%9E%B6)** | **[🐂<br>大牛一览表](https://github.com/0voice/Understanding_in_Rust#-%E5%A4%A7%E7%89%9B%E4%B8%80%E8%A7%88%E8%A1%A8)**
  
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
  

# ✈ 杂货铺
  
- Rust 最大中文社区论坛：https://rustcc.cn/
- 小众中文社区的翻译资料/论坛：https://learnku.com/rust
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
  
  
  
# 🐂 大牛语录

## 联系专栏

#### 零声教育，专注于c/c++Linux后台服务器开发架构技术学习提升。<br>
每天晚上8点【免费技术直播】：[分享Linux，Nginx，ZeroMQ，MySQL，Redis，fastdfs，MongoDB，ZK，流媒体，CDN，P2P，K8S，Docker，TCP/IP，协程，DPDK等技术内容，立即学习。](https://ke.qq.com/course/417774?flowToken=1037711)

#### 关注微信公众号【后台服务架构师】——【联系我们】，获取本repo最全PDF学习文档！

<img width="65%" height="65%" src="https://user-images.githubusercontent.com/87457873/130796999-03af3f54-3719-47b4-8e41-2e762ab1c68b.png"/>
  
  
  
  
  
