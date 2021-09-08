# 🏄💨Rust工程师枕边资料，经典博客，大牛文章，开源框架，论文，视频，书籍，作者口述一览表

<div align=center>

![rust](https://user-images.githubusercontent.com/87457873/132184451-55f1125e-acad-4cc7-9e56-ecbffc0db412.png)
  
## 一个安全、并发、实用的系统语言

<br>
<br>
  
   [🏝<br>&nbsp;&nbsp;&nbsp; &nbsp;环境搭建&nbsp;&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E7%8E%AF%E5%A2%83%E6%90%AD%E5%BB%BA)  |[📕<br>&nbsp;&nbsp;&nbsp; 入门秘笈&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88-pdf%E6%A1%A3%E4%B8%8B%E8%BD%BD)|  [📖<br>&nbsp;&nbsp;&nbsp; 电子书籍&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E4%B9%A6%E7%B1%8D)
:-------: | :-------: | :---------:
 **[📑<br>大牛文章](https://github.com/0voice/Understanding_in_Rust#-%E5%A4%A7%E7%89%9B%E6%96%87%E7%AB%A0)**  |  **[📰<br>论文](https://github.com/0voice/Understanding_in_Rust#-%E8%AE%BA%E6%96%87)**|  **[✈<br> 杂货铺](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E6%9D%82%E8%B4%A7%E9%93%BA)**
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

# 📖 书籍
 
> 以下电子书籍，仅供学习参考。
  
- [《Rust编程之道》](https://www.aliyundrive.com/s/4vMVLw3CgzH)
  
- [《深入浅出Rust》](https://www.aliyundrive.com/s/2HdYEootmWH)
  
- [《Rust权威指南》](https://www.aliyundrive.com/s/wUXm3x7fCnW)
  
- [《Rust 程序设计语言》](https://www.aliyundrive.com/s/UNQm1AvMQTR)
  
- [《精通Rust(第2版)》](https://www.aliyundrive.com/s/mgzphhMbbX1)
   
  
# 📑 大牛文章
  
- [华为 | 可信编程 -- 华为引领Rust语言开发的实践和愿景](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E5%8D%8E%E4%B8%BA%20%7C%20%E5%8F%AF%E4%BF%A1%E7%BC%96%E7%A8%8B%20--%20%E5%8D%8E%E4%B8%BA%E5%BC%95%E9%A2%86Rust%E8%AF%AD%E8%A8%80%E5%BC%80%E5%8F%91%E7%9A%84%E5%AE%9E%E8%B7%B5%E5%92%8C%E6%84%BF%E6%99%AF.md)

- [华为 | 基于Rust的下一代虚拟化平台-StratoVirt](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E5%8D%8E%E4%B8%BA%20%7C%20%E5%9F%BA%E4%BA%8ERust%E7%9A%84%E4%B8%8B%E4%B8%80%E4%BB%A3%E8%99%9A%E6%8B%9F%E5%8C%96%E5%B9%B3%E5%8F%B0-StratoVirt.md)
  
- [Rust中的错误传递和日志记录](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/Rust%E4%B8%AD%E7%9A%84%E9%94%99%E8%AF%AF%E4%BC%A0%E9%80%92%E5%92%8C%E6%97%A5%E5%BF%97%E8%AE%B0%E5%BD%95.md)

- [io_uring | 用 Rust 实现基于 io_uring 的异步随机读文件](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/io_uring%20%7C%20%E7%94%A8%20Rust%20%E5%AE%9E%E7%8E%B0%E5%9F%BA%E4%BA%8E%20io_uring%20%E7%9A%84%E5%BC%82%E6%AD%A5%E9%9A%8F%E6%9C%BA%E8%AF%BB%E6%96%87%E4%BB%B6.md)

- [「译」使用 Rust 实现命令行生命游戏](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E3%80%8C%E8%AF%91%E3%80%8D%E4%BD%BF%E7%94%A8%20Rust%20%E5%AE%9E%E7%8E%B0%E5%91%BD%E4%BB%A4%E8%A1%8C%E7%94%9F%E5%91%BD%E6%B8%B8%E6%88%8F.md)

- [图解 Rust 所有权与生命周期](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E5%9B%BE%E8%A7%A3%20Rust%20%E6%89%80%E6%9C%89%E6%9D%83%E4%B8%8E%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F.md)

- [蚂蚁集团 CeresDB 团队 | 关于 Rust 错误处理的思考](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E8%9A%82%E8%9A%81%E9%9B%86%E5%9B%A2%20CeresDB%20%E5%9B%A2%E9%98%9F%20%7C%20%E5%85%B3%E4%BA%8E%20Rust%20%E9%94%99%E8%AF%AF%E5%A4%84%E7%90%86%E7%9A%84%E6%80%9D%E8%80%83.md)

- [解读 Rust 1.50 稳定版](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E8%A7%A3%E8%AF%BB%20Rust%201.50%20%E7%A8%B3%E5%AE%9A%E7%89%88.md)


  
# 📰 论文
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
  
### Observability

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
  
# 🐂 大牛一览表
