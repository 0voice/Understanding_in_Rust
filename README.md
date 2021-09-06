# 🏄💨Rust工程师枕边资料，经典博客，大牛文章，开源框架，国外项目，论文，视频，书籍，作者口述一览表

<div align=center>

![rust](https://user-images.githubusercontent.com/87457873/132184451-55f1125e-acad-4cc7-9e56-ecbffc0db412.png)
  
## 一个安全、并发、实用的系统语言

<br>
<br>
  
   [🏝<br>&nbsp;&nbsp;&nbsp; &nbsp;环境搭建&nbsp;&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E7%8E%AF%E5%A2%83%E6%90%AD%E5%BB%BA)  |[📕<br>&nbsp;&nbsp;&nbsp; 入门秘笈&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88)|  [📖<br>&nbsp;&nbsp;&nbsp; 电子书籍&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E4%B9%A6%E7%B1%8D)
:-------: | :-------: | :---------:
 **[📑<br>大牛文章](https://github.com/0voice/Understanding_in_Rust#-%E5%A4%A7%E7%89%9B%E6%96%87%E7%AB%A0)**  |  **[📰<br>论文](https://github.com/0voice/Understanding_in_Rust#-%E8%AE%BA%E6%96%87)**|  **[✈<br> 国外项目](https://github.com/0voice/Understanding_in_Rust#-%E5%9B%BD%E5%A4%96%E9%A1%B9%E7%9B%AE)**
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

# 📕 入门秘笈

### Rust教学

#### Rust是什么？

- Rust是由Mozilla员工「Graydon Hoare」于2006年开发的系统程式设计语言。他将这种语言描述为支援功能和命令正规化的「安全，并行和实用的语言」。
- Rust的语法类似于C++语言。
- Rust是免费的开源软体，即任何人都可以自由使用该软体，并且公开共用原始码，以便人们也可以改进软体的设计。
- Rust在2016年，2017年和2018年的堆叠溢位开发者调查中被宣布为「最受欢迎的程式设计语言」之一。
- 没有像 这意味着，记忆体由Rust内部管理。`calloc``malloc`

#### Rust的使用者有哪些？

出于多种原因，Rust语言对许多人来说是理想的。

下面来看看吧：

- **开发团队 低阶程式设计程式码包含需要测试人员进行大量测试的错误。但是，在Rust的情况下，如果程式包含错误，编译器拒绝编译程式码。通过与编译器并行工作，开发人员可以专注于程式的逻辑而不是专注于错误。**
- **学生 Rust团队正在努力使普通人更容易理解系统概念，特别是那些不熟悉程式设计的人。**
- **公司 这些任务包括命令列工具，Web服务，DevOps工具，嵌入式装置，音讯和视讯分析和转码，加密货币，生物资讯学，搜寻引擎，物联网应用程式，机器学习，甚至Firefox Web浏览器的重要部分。**
- **开源开发人员 因此，他们可以使用原始码来改进Rust的设计。**

## 面向读者

此Rust教学旨在帮助初学者和专业人士快速了解学习并熟悉Rust语言的程式设计知识和应用。

#### [Rust简介]()
#### [Rust的特点]()
#### [Rust开发环境安装]()
#### [Rust第一个程式]()
#### [Rust if语句]()
#### [Rust if in a let语句]()
#### [Rust loop回圈]()
#### [Rust for回圈]()
#### [Rust while回圈]()
#### [Rust参照和借用]()
#### [Rust结构体]()
#### [Rust结构体更新语法]()
#### [Rust结构体方法语法]()
#### [Rust列举]()
#### [匹配运算子]()
#### [Rust if let控制流程]()
#### [Rust档案系统]()
#### [Rust公开函式]()
#### [Rust use关键字参照模组]()
#### [Rust向量]()
#### [Rust字串]()
#### [Rust错误处理]()
#### [Rust不可恢复的错误]()
#### [Rust可恢复的错误]()
#### [Rust泛型]()
#### [Rust Trait]()
#### [Rust生命周期]()
#### [Rust智慧指标]()
#### [Rust Box<T>]()
#### [Rust Deref trait]()
#### [Rust Drop trait]()


# 📖 书籍
# 📑 大牛文章
# 📰 论文
# 💽 视频
# 🏗 开源框架
# ✈ 国外项目
# 🐂 大牛一览表
