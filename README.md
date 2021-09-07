# 🏄💨Rust工程师枕边资料，经典博客，大牛文章，开源框架，国外项目，论文，视频，书籍，作者口述一览表

<div align=center>

![rust](https://user-images.githubusercontent.com/87457873/132184451-55f1125e-acad-4cc7-9e56-ecbffc0db412.png)
  
## 一个安全、并发、实用的系统语言

<br>
<br>
  
   [🏝<br>&nbsp;&nbsp;&nbsp; &nbsp;环境搭建&nbsp;&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E7%8E%AF%E5%A2%83%E6%90%AD%E5%BB%BA)  |[📕<br>&nbsp;&nbsp;&nbsp; 入门秘笈&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88-pdf%E6%A1%A3%E4%B8%8B%E8%BD%BD)|  [📖<br>&nbsp;&nbsp;&nbsp; 电子书籍&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E4%B9%A6%E7%B1%8D)
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

# 📕 入门秘笈 [（PDF档下载）](https://github.com/0voice/Understanding_in_Rust/blob/main/Rust%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88.pdf)

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

[Rust简介](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%AE%80%E4%BB%8B.md)<br>
[Rust的特点](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%9A%84%E7%89%B9%E7%82%B9.md)<br>
[Rust开发环境安装](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83%E5%AE%89%E8%A3%85.md)<br>
[Rust第一个程式](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%AC%AC%E4%B8%80%E4%B8%AA%E7%A8%8B%E5%BC%8F.md)<br>
[Rust if语句](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20if%E8%AF%AD%E5%8F%A5.md)<br>
[Rust if in a let语句](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20if%20in%20a%20let%E8%AF%AD%E5%8F%A5.md)<br>
[Rust loop回圈](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20loop%E5%9B%9E%E5%9C%88.md)<br>
[Rust for回圈](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20for%E5%9B%9E%E5%9C%88.md)<br>
[Rust while回圈](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20while%E5%9B%9E%E5%9C%88.md)<br>
[Rust所有权](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%89%80%E6%9C%89%E6%9D%83.md)<br>
[Rust参照和借用](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%8F%82%E7%85%A7%E5%92%8C%E5%80%9F%E7%94%A8.md)<br>
[Rust切片](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%88%87%E7%89%87.md)<br>
[Rust结构体](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%BB%93%E6%9E%84%E4%BD%93.md)<br>
[Rust结构体更新语法](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%BB%93%E6%9E%84%E4%BD%93%E6%9B%B4%E6%96%B0%E8%AF%AD%E6%B3%95.md)<br>
[Rust结构体方法语法](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%BB%93%E6%9E%84%E4%BD%93%E6%96%B9%E6%B3%95%E8%AF%AD%E6%B3%95.md)<br>
[Rust列举](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%88%97%E4%B8%BE.md)<br>
[匹配运算子](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/%E5%8C%B9%E9%85%8D%E8%BF%90%E7%AE%97%E5%AD%90.md)<br>
[Rust if let控制流程](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20if%20let%E6%8E%A7%E5%88%B6%E6%B5%81%E7%A8%8B.md)<br>
[Rust模组](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%A8%A1%E7%BB%84.md)<br>
[Rust档案系统](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%A1%A3%E6%A1%88%E7%B3%BB%E7%BB%9F.md)<br>
[Rust公开函式](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%85%AC%E5%BC%80%E5%87%BD%E5%BC%8F.md)<br>
[Rust use关键字参照模组](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20use%E5%85%B3%E9%94%AE%E5%AD%97%E5%8F%82%E7%85%A7%E6%A8%A1%E7%BB%84.md)<br>
[Rust向量](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%90%91%E9%87%8F.md)<br>
[Rust字串](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%AD%97%E4%B8%B2.md)<br>
[Rust错误处理](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E9%94%99%E8%AF%AF%E5%A4%84%E7%90%86.md)
[Rust不可恢复的错误](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E4%B8%8D%E5%8F%AF%E6%81%A2%E5%A4%8D%E7%9A%84%E9%94%99%E8%AF%AF.md)<br>
[Rust可恢复的错误](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%8F%AF%E6%81%A2%E5%A4%8D%E7%9A%84%E9%94%99%E8%AF%AF.md)<br>
[Rust泛型](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%B3%9B%E5%9E%8B.md)<br>
[Rust Trait](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Trait.md)<br>
[Rust生命周期](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F.md)<br>
[Rust智慧指标](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%99%BA%E6%85%A7%E6%8C%87%E6%A0%87.md)<br>
[Rust Box<T>](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Box%3CT%3E.md)<br>
[Rust Deref trait](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Deref%20trait.md)<br>
[Rust Drop trait](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Drop%20trait.md)<br>

# 📖 书籍
  
[《Rust编程之道》](https://www.aliyundrive.com/s/4vMVLw3CgzH)
  
[《深入浅出Rust》](https://www.aliyundrive.com/s/2HdYEootmWH)
  
[《Rust权威指南》](https://www.aliyundrive.com/s/wUXm3x7fCnW)
  
[《Rust 程序设计语言》](https://www.aliyundrive.com/s/UNQm1AvMQTR)
  
[《精通Rust(第2版)》](https://www.aliyundrive.com/s/mgzphhMbbX1)
   
  
# 📑 大牛文章
  
[华为 | 可信编程 -- 华为引领Rust语言开发的实践和愿景](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E5%8D%8E%E4%B8%BA%20%7C%20%E5%8F%AF%E4%BF%A1%E7%BC%96%E7%A8%8B%20--%20%E5%8D%8E%E4%B8%BA%E5%BC%95%E9%A2%86Rust%E8%AF%AD%E8%A8%80%E5%BC%80%E5%8F%91%E7%9A%84%E5%AE%9E%E8%B7%B5%E5%92%8C%E6%84%BF%E6%99%AF.md)

[华为 | 基于Rust的下一代虚拟化平台-StratoVirt](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E5%8D%8E%E4%B8%BA%20%7C%20%E5%9F%BA%E4%BA%8ERust%E7%9A%84%E4%B8%8B%E4%B8%80%E4%BB%A3%E8%99%9A%E6%8B%9F%E5%8C%96%E5%B9%B3%E5%8F%B0-StratoVirt.md)
  
[Rust中的错误传递和日志记录](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/Rust%E4%B8%AD%E7%9A%84%E9%94%99%E8%AF%AF%E4%BC%A0%E9%80%92%E5%92%8C%E6%97%A5%E5%BF%97%E8%AE%B0%E5%BD%95.md)

[io_uring | 用 Rust 实现基于 io_uring 的异步随机读文件](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/io_uring%20%7C%20%E7%94%A8%20Rust%20%E5%AE%9E%E7%8E%B0%E5%9F%BA%E4%BA%8E%20io_uring%20%E7%9A%84%E5%BC%82%E6%AD%A5%E9%9A%8F%E6%9C%BA%E8%AF%BB%E6%96%87%E4%BB%B6.md)

[「译」使用 Rust 实现命令行生命游戏](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E3%80%8C%E8%AF%91%E3%80%8D%E4%BD%BF%E7%94%A8%20Rust%20%E5%AE%9E%E7%8E%B0%E5%91%BD%E4%BB%A4%E8%A1%8C%E7%94%9F%E5%91%BD%E6%B8%B8%E6%88%8F.md)

[图解 Rust 所有权与生命周期](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E5%9B%BE%E8%A7%A3%20Rust%20%E6%89%80%E6%9C%89%E6%9D%83%E4%B8%8E%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F.md)

[蚂蚁集团 CeresDB 团队 | 关于 Rust 错误处理的思考](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E8%9A%82%E8%9A%81%E9%9B%86%E5%9B%A2%20CeresDB%20%E5%9B%A2%E9%98%9F%20%7C%20%E5%85%B3%E4%BA%8E%20Rust%20%E9%94%99%E8%AF%AF%E5%A4%84%E7%90%86%E7%9A%84%E6%80%9D%E8%80%83.md)

[解读 Rust 1.50 稳定版](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E8%A7%A3%E8%AF%BB%20Rust%201.50%20%E7%A8%B3%E5%AE%9A%E7%89%88.md)


  
# 📰 论文
# 💽 视频
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
  
  
# ✈ 国外项目
# 🐂 大牛一览表
