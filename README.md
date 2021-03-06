# ðð¨ãæå®å¨çç¼ç¨è¯­è¨ãRustå·¥ç¨å¸æè¾¹èµæï¼å¤§çæç« ï¼å¼æºæ¡æ¶ï¼å®æ¹ææ¡£ï¼è§é¢ï¼æ¨èä¹¦ç±ï¼å­¦ä¹ å¹²è´§ï¼å¤§çè¯­å½

<div align=center>

![rust](https://user-images.githubusercontent.com/87457873/132184451-55f1125e-acad-4cc7-9e56-ecbffc0db412.png)
  
## ä¸ä¸ªå®å¨ãå¹¶åãå®ç¨çç³»ç»è¯­è¨

<br>
<br>
  
   [ð<br>&nbsp;&nbsp;&nbsp; &nbsp;ç¯å¢æ­å»º&nbsp;&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E7%8E%AF%E5%A2%83%E6%90%AD%E5%BB%BA)  |[ð<br>&nbsp;&nbsp;&nbsp; å¥é¨ç§ç¬&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust#-%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88-pdf%E6%A1%A3%E4%B8%8B%E8%BD%BD)|  [ð<br>&nbsp;&nbsp;&nbsp; æ¨èä¹¦ç±&nbsp;&nbsp;&nbsp; ](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E6%8E%A8%E8%8D%90%E4%B9%A6%E7%B1%8D)
:-------: | :-------: | :---------:
 **[ð<br>ç²¾éæç« ](https://github.com/0voice/Understanding_in_Rust#-%E5%A4%A7%E7%89%9B%E6%96%87%E7%AB%A0)**  |  **[ð°<br>å®æ¹ææ¡£](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E5%AE%98%E6%96%B9%E6%96%87%E6%A1%A3)**|  **[â<br> æè´§éº](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E6%9D%82%E8%B4%A7%E9%93%BA)**
**[ð½<br>è§é¢](https://github.com/0voice/Understanding_in_Rust#-%E8%A7%86%E9%A2%91)** | **[ð<br>å¼æºæ¡æ¶](https://github.com/0voice/Understanding_in_Rust#-%E5%BC%80%E6%BA%90%E6%A1%86%E6%9E%B6)** | **[ð<br>å¤§çè¯­å½](https://github.com/0voice/Understanding_in_Rust/blob/main/README.md#-%E5%A4%A7%E7%89%9B%E8%AF%AD%E5%BD%95)**
  
<br>
<br>  

</div>




# ð¤ Why Rustï¼Why canï¼

### Jay Oster, PubNub æ¶æå¸ :

âé¤äºå®å¨åæ§è½ï¼æä»¬è¿æï¼

- æ³åï¼
- ç¹å¾ï¼
- ä»£æ°ç±»åï¼
- å½æ°å¼åå½ä»¤å¼èå¼ï¼
- å¯è½æ¯ä¸çä¸æå¥½çä¾èµç®¡çåæå»ºå·¥å·ï¼å®éä¸è§£å³äºâä¾èµå°ç±âé®é¢ï¼
- å¯¹ååµææ¡£ãæµè¯åæ§è½è¯æµçç¾å¦æ¯æï¼
- ä¸ä¸ªå¤§çä¸æ­£å¨çé¿çåºãæ½è±¡ãå·¥å·çæï¼
- è¿ç¨å®ï¼
- ä¸å·²æä»£ç ç FFI äº¤äºæ§ï¼
- æ¯æä¸æå¹³å°ï¼æ´å¤çå¨è·¯ä¸ï¼ï¼ï¼
- å¯¹å¼åèä½éªæ¯æ­£åçãæ¯åº¸ç½®ççæ»¡è¶³ã

Rust æ¯å¯ä¸ä¸ä¸ªä¸é¢æææ¡æ¡é½æå¾çè¯­è¨ï¼

- åå­å®å¨
- ç±»åå®å¨
- æ¶é¤æ°æ®ç«äº
- ä½¿ç¨åç¼è¯
- å»ºç«ï¼å¹¶ä¸é¼å±ï¼å¨é¶æ½è±¡ä¹ä¸
- æå°çè¿è¡æ¶ï¼æ åæ­¢ä¸ççåå¾æéå¨ï¼æ  JIT ç¼è¯å¨ï¼æ  VMï¼
- ä½åå­å ç¨ï¼ç¨åºå¯ä»¥è¿è¡å¨èµæºåéçç¯å¢ï¼æ¯å¦å°çå¾®æ§å¶å¨ï¼
- è£¸éå±ç®æ ï¼æ¯å¦ï¼åä¸ä¸ª OS åæ ¸æèè®¾å¤é©±å¨ï¼æ Rust å½ä¸ä¸ª âé«å±âæ±ç¼å¨ä½¿ç¨ï¼â

### Peter Varo:

âRust æä¸ä¸ªå¾é¦çå°æ¹ï¼å®å C å C++ é£æ ·åºå±ï¼å æ­¤ä¹å·æåºå±çè¿äºä¼å¿ï¼æ¯å¦ï¼æ§å¶ãå¤§å°ãéåº¦ç­ï¼ãåæ¶å¢ï¼å®åå Haskell é£æ ·é«å±ï¼èªå¸¦ä»¤äººåæçå¤§éåè½ä¼ æ¿ãå®è¿æ¯å½ä»¤å¼çï¼æä»¥å®¹æè¢«å¤§å¤æ°äººä¸æãç¶åå®åå Python ä¸æ ·çµæ´»ï¼æ¯å¦ï¼' é¸­å­ç±»åï¼duck-typingï¼' çæ¦å¿µåºç°å¨ç¼è¯æ¶ï¼æ¯å¦ï¼ç¹å¾éå®ï¼ï¼ç¶åå®åæ²¡æéæ§çé¢åå¯¹è±¡æ¨¡åä»¥åç±è¿ä¸ªæ¨¡åå¯¼è´çåç§åºåçé®é¢ã

æåä½å¾éè¦çæ¯ï¼è¿æä¸è¿ä¸²çä¸è¥¿è¢«åå«è¿æ¥ï¼ç²¾ç®ç­å°çè¯­æ³ï¼è¯­è¨æä¾çæ°ç®ä¸å¤çç¹æ§ï¼æ ååºåå¶ä¸è´æ§ï¼é«è´¨éçææ¡£çéæï¼åæ¬å¯¹åå­¦èåé«çº§ç¨æ·é½éç¨çå­¦ä¹ ææï¼è¿äºé½æ¯ä¿æå ç´ ãâ

# ð ç¯å¢æ­å»º

**å®è£åå·¥å·ï¼https://www.rust-lang.org/zh-CN/learn/get-started**

# ð å¥é¨ç§ç¬ [ï¼PDFæ¡£ä¸è½½ï¼](https://github.com/0voice/Understanding_in_Rust/blob/main/Rust%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88.pdf)

- [Rustç®ä»](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%AE%80%E4%BB%8B.md)<br>
- [Rustçç¹ç¹](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%9A%84%E7%89%B9%E7%82%B9.md)<br>
- [Rustå¼åç¯å¢å®è£](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83%E5%AE%89%E8%A3%85.md)<br>
- [Rustç¬¬ä¸ä¸ªç¨å¼](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%AC%AC%E4%B8%80%E4%B8%AA%E7%A8%8B%E5%BC%8F.md)<br>
- [Rust ifè¯­å¥](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20if%E8%AF%AD%E5%8F%A5.md)<br>
- [Rust if in a letè¯­å¥](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20if%20in%20a%20let%E8%AF%AD%E5%8F%A5.md)<br>
- [Rust loopåå](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20loop%E5%9B%9E%E5%9C%88.md)<br>
- [Rust foråå](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20for%E5%9B%9E%E5%9C%88.md)<br>
- [Rust whileåå](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20while%E5%9B%9E%E5%9C%88.md)<br>
- [Rustæææ](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%89%80%E6%9C%89%E6%9D%83.md)<br>
- [Ruståç§ååç¨](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%8F%82%E7%85%A7%E5%92%8C%E5%80%9F%E7%94%A8.md)<br>
- [Ruståç](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%88%87%E7%89%87.md)<br>
- [Rustç»æä½](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%BB%93%E6%9E%84%E4%BD%93.md)<br>
- [Rustç»æä½æ´æ°è¯­æ³](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%BB%93%E6%9E%84%E4%BD%93%E6%9B%B4%E6%96%B0%E8%AF%AD%E6%B3%95.md)<br>
- [Rustç»æä½æ¹æ³è¯­æ³](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%BB%93%E6%9E%84%E4%BD%93%E6%96%B9%E6%B3%95%E8%AF%AD%E6%B3%95.md)<br>
- [Ruståä¸¾](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%88%97%E4%B8%BE.md)<br>
- [å¹éè¿ç®å­](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/%E5%8C%B9%E9%85%8D%E8%BF%90%E7%AE%97%E5%AD%90.md)<br>
- [Rust if letæ§å¶æµç¨](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20if%20let%E6%8E%A7%E5%88%B6%E6%B5%81%E7%A8%8B.md)<br>
- [Rustæ¨¡ç»](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%A8%A1%E7%BB%84.md)<br>
- [Rustæ¡£æ¡ç³»ç»](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%A1%A3%E6%A1%88%E7%B3%BB%E7%BB%9F.md)<br>
- [Rustå¬å¼å½å¼](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%85%AC%E5%BC%80%E5%87%BD%E5%BC%8F.md)<br>
- [Rust useå³é®å­åç§æ¨¡ç»](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20use%E5%85%B3%E9%94%AE%E5%AD%97%E5%8F%82%E7%85%A7%E6%A8%A1%E7%BB%84.md)<br>
- [Ruståé](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%90%91%E9%87%8F.md)<br>
- [Rustå­ä¸²](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%AD%97%E4%B8%B2.md)<br>
- [Rustéè¯¯å¤ç](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E9%94%99%E8%AF%AF%E5%A4%84%E7%90%86.md)
- [Rustä¸å¯æ¢å¤çéè¯¯](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E4%B8%8D%E5%8F%AF%E6%81%A2%E5%A4%8D%E7%9A%84%E9%94%99%E8%AF%AF.md)<br>
- [Rustå¯æ¢å¤çéè¯¯](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E5%8F%AF%E6%81%A2%E5%A4%8D%E7%9A%84%E9%94%99%E8%AF%AF.md)<br>
- [Rustæ³å](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%B3%9B%E5%9E%8B.md)<br>
- [Rust Trait](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Trait.md)<br>
- [Rustçå½å¨æ](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F.md)<br>
- [Rustæºæ§ææ ](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%E6%99%BA%E6%85%A7%E6%8C%87%E6%A0%87.md)<br>
- [Rust Box<T>](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Box%3CT%3E.md)<br>
- [Rust Deref trait](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Deref%20trait.md)<br>
- [Rust Drop trait](https://github.com/0voice/Understanding_in_Rust/blob/main/%E5%85%A5%E9%97%A8%E7%A7%98%E7%AC%88/Rust%20Drop%20trait.md)<br>

# ð æ¨èä¹¦ç±
  
### å½åä¹¦ç±
  
- [ãæ·±å¥æµåºRustã](https://jp1lib.org/s/?q=%E3%80%8A%E6%B7%B1%E5%85%A5%E6%B5%85%E5%87%BARust%E3%80%8B)
  
- [ãRustæå¨æåã](https://book.douban.com/subject/35081743/)
  
- [ãRust ç¨åºè®¾è®¡è¯­è¨ã](https://kaisery.github.io/trpl-zh-cn/)
  
- [ãç²¾éRust(ç¬¬2ç)ã](https://jp1lib.org/book/17127064/820864)
  
### å½å¤ä¹¦ç±
  
**å¥é¨ä¹¦ç±**
  
- [ãThe Rust Programming Languageã](https://doc.rust-lang.org/book/)
  
æ¬¢è¿ï¼æ¬ä¹¦å°æä½ æå³ Rust ç¼ç¨è¯­è¨çç¥è¯ãRust æ¯ä¸ç§ç³»ç»ç¼ç¨è¯­è¨ï¼ä¸æ³¨äºä¸ä¸ªç®æ ï¼å®å¨æ§ãéåº¦åå¹¶åæ§ãå®å¨æ²¡æåå¾æ¶éå¨çæåµä¸å®ç°äºè¿äºç®æ ï¼ä½¿å¶æä¸ºå¶ä»è¯­è¨ä¸æé¿çè®¸å¤ç¨ä¾çæç¨è¯­è¨ï¼åµå¥å¶ä»è¯­è¨ãå·æç¹å®ç©ºé´åæ¶é´è¦æ±çç¨åºä»¥åç¼åä½çº§ä»£ç ï¼ä¾å¦è®¾å¤é©±å¨ç¨åºåæä½ç³»ç»ãå®éè¿å¨ä¸äº§çè¿è¡æ¶å¼éçæåµä¸è¿è¡å¤§éç¼è¯æ¶å®å¨æ£æ¥ï¼åæ¶æ¶é¤æææ°æ®ç«äºï¼ä»èæ¹è¿äºéå¯¹æ­¤ç©ºé´çå½åè¯­è¨ãRust è¿æ¨å¨å®ç°âé¶ææ¬æ½è±¡âï¼å°½ç®¡å¶ä¸­ä¸äºæ½è±¡æè§åæ¯é«çº§è¯­è¨çæ½è±¡ãå³ä¾¿å¦æ­¤ï¼Rust ä»ç¶åè®¸åä½çº§è¯­è¨ä¸æ ·è¿è¡ç²¾ç¡®æ§å¶ã
  
- [ãWelcome to Rust-101ã](https://www.ralfj.de/projects/rust-101/main.html)
  
è¿æ¯ Rust-101ï¼ä¸ä¸ª Rust è¯­è¨çå°æç¨ãå®æ¨å¨æä¸ºä¸é¨äº¤äºå¼çå¨æè¯¾ç¨ï¼æç¸ä¿¡çæ­£å­¦ä¹ ä¸é¨è¯­è¨çå¯ä¸æ¹æ³æ¯å¨å¶ä¸­ç¼åä»£ç ï¼å æ­¤æ¨åºè¯¥å¨è¯¾ç¨ä¸­è¿è¡ç¼ç ãå¦ææ¨æä»»ä½æªå¨æ­¤å¤åç­çé®é¢ï¼è¯·æ¥çä¸é¢çâå¶ä»èµæºâãå°¤å¶æ¯ï¼IRC é¢ééæ¤æ»¡äºæ¿æå¸®å©ä½ çå¾æ£çäººï¼æå¨é£éè±äºå¾å¤æ¶é´ ;-) æåè®¾å¯¹ç¼ç¨æä¸å®çäºè§£ï¼å æ­¤ä¸ä¼è§£éå¤§å¤æ°è¯­è¨å±æçåºæ¬æ¦å¿µãç¸åï¼æå°ä¸æ³¨äº Rust çç¹æ®ä¹å¤ã
  
- [ãRust by Exampleã](http://rustbyexample.com/)
  
Rust by Example (RBE) æ¯ä¸ç»å¯è¿è¡çç¤ºä¾ï¼ç¨äºè¯´æåç§ Rust æ¦å¿µåæ ååºã
  
- [ãWhy Rust?ã](https://kr1lib.org/book/10990507/3a18af) 
  
å°½ç®¡èª 40 å¤å¹´åå¼å¥ C ä»¥æ¥ï¼ç³»ç»ç¼ç¨è¯­è¨å·²ç»æäºå¾å¤§çåå±ï¼ä½æä»¬å¯¹é æå·¨å¤§åæçæè ¢éè¯¯çè½åä»ç¶æ²¡ææ¹åï¼æ°é»ä¸­ç»å¸¸æçå¨çä¾å­ãè¿ä»½ O'Reilly æ¥åç ç©¶äº Rustï¼è¿æ¯ä¸ç§æ°çç³»ç»ç¼ç¨è¯­è¨ï¼å®å°å®å¨æ§åå®å¨æ§ä¸æ§è½ç¸ç»åï¼ä¸ C å C++ ç¸å½ã
  
- [ãLearning Rustã](https://kr1lib.org/book/11689651/08c0b6) 
  
Rust æ¯ä¸ç§é«åº¦å¹¶ååé«æ§è½çè¯­è¨ï¼ä¸æ³¨äºå®å¨åéåº¦ãåå­ç®¡çåç¼åå¹²åçä»£ç ãå®è¿ä¿è¯çº¿ç¨å®å¨ï¼å¶ç®çæ¯æé«ç°æåºç¨ç¨åºçæ§è½ãå®å¾å°äº Mozilla çæ¯æï¼ä»¥è§£å³å¹¶åçå³é®é®é¢ã 
  
- [ãBeginning Rust - From Novice to Professionalã](https://kr1lib.org/book/3490555/7b7c82)
  
å­¦ä¹ å¨ UnixãLinux shellãmacOS å Windows å½ä»¤è¡ä¸ä»¥ç®åãå¾ªåºæ¸è¿çæ¹å¼ä½¿ç¨ Rust è¿è¡ç¼ç¨ãå½æ¨éè¯»æ¬ä¹¦æ¶ï¼æ¨å°å»ºç«å¨æ¨å¨åå ç« ä¸­è·å¾çç¥è¯çåºç¡ä¸ï¼å¹¶äºè§£ Rust æä¾äºä»ä¹ã

å¼å§ Rust ä» Rust çåºç¡å¼å§ï¼åæ¬å¦ä½å½åå¯¹è±¡ãæ§å¶æ§è¡æµåå¤çåå§ç±»åãæ¨å°çå°å¦ä½è¿è¡ç®æ¯è¿ç®ãåéåå­ãä½¿ç¨è¿­ä»£å¨ä»¥åå¤çè¾å¥/è¾åºãä¸æ¦ææ¡äºè¿äºæ ¸å¿æè½ï¼æ¨å°çæå¤çéè¯¯å¹¶ä½¿ç¨ Rust çé¢åå¯¹è±¡ç¹æ§ç«å³æå»ºå¥å£®ç Rust åºç¨ç¨åºã

åªéè¦åºæ¬çç¼ç¨ç¥è¯ï¼æå¥½æ¯ C æ C++ãè¦çè§£è¿æ¬ä¹¦ï¼ç¥éä»ä¹æ¯æ´æ°åæµ®ç¹æ°ï¼ä»¥ååºåæ è¯ç¬¦åå­ç¬¦ä¸²æå­å°±è¶³å¤äºã
  
- [ãRust Cookbookã](https://kr1lib.org/book/3362654/66eb5a)  
  
æ¬ä¹¦å°å¸®å©æ¨çè§£ Rust è¯­è¨çæ ¸å¿æ¦å¿µï¼ä½¿æ¨è½å¤éè¿æ´åé¶ææ¬æ½è±¡åæ´å¥½çåå­ç®¡çç­åè½æ¥å¼åé«æåé«æ§è½çåºç¨ç¨åºãæ·±å¥ç ç©¶ Rust ä¸­çé«çº§æ¦å¿µï¼ä¾å¦éè¯¯å¤çãå®ãååå¹¶è¡æ§ãå¨æ¬ä¹¦çæåï¼å­¦ä¹ å¦ä½åå»º HTTP æå¡å¨å Web æå¡ï¼å¨æå¡å¨ç«¯ç¼ç¨æ¹é¢å»ºç«å¼ºå¤§çåºç¡ç¥è¯ï¼å¹¶è½å¤æä¾ä½¿ç¨ Rust æå»ºé«æ§è½åæ´å®å¨ççäº§çº§ Web åºç¨ç¨åºåæå¡çè§£å³æ¹æ¡ã
  
- [ãRust Standard Library Cookbookã](https://kr1lib.org/book/3571952/9b9cdb)  
  
Mozilla ç Rust ä»¥å¶æäººçåè½åå¼ºå¤§çåºèå¤åå³æ³¨ãæ¬ä¹¦å°å¸¦æ¨äºè§£åç§ç§è¯ï¼ææ¨å¦ä½å©ç¨æ ååºæ¥å®ç°é«æçè§£å³æ¹æ¡ã

æ¬ä¹¦é¦åç®è¦ä»ç»äºæ ååºåé¦èçåºæ¬æ¨¡åãä»è¿éå¼å§ï¼é£è°±å°æ¶µçéè¿è§£ææ¯ææä»¶/ç®å½å¤çåäº¤äºçåãæ¨å°äºè§£ä¸é«çº§æ°æ®ç»æãéè¯¯å¤çåç½ç»ç¸å³çåãæ¨è¿å°å­¦ä¹ ä½¿ç¨æè´§åå®éªæ§å¤é´åè½ãè¿æ¬ä¹¦è¿æ¶µçäº Rust ä¸­æç¸å³çå¤é¨ crateã
  
- [ãNetwork Programming with Rustã](https://kr1lib.org/book/3571947/48c564)  
  
Rust è¶³å¤ä½çº§ï¼å¯ä»¥æä¾å¯¹åå­çç»ç²åº¦æ§å¶ï¼åæ¶éè¿ç¼è¯æ¶éªè¯æä¾å®å¨æ§ãè¿ä½¿å¾å®ç¹å«éåç¼åä½çº§ç½ç»åºç¨ç¨åºã

æ¬ä¹¦åä¸ºä¸ä¸ªä¸»è¦é¨åï¼å°å¸¦æ¨è¸ä¸æå»ºåè½é½å¨ç Web æå¡å¨çæ¿å¨äººå¿çæç¨ãæ¬ä¹¦é¦åå¯¹ Rust ååºæ¬çç½ç»æ¦å¿µè¿è¡äºæå®çä»ç»ãè¿å°ä¸ºæ´æ¬ä¹¦å¥ å®åºç¡å¹¶å®ä¸åºè°ãå¨ç¬¬äºé¨åä¸­ï¼æä»¬å°æ·±å¥ç ç©¶å¦ä½ä½¿ç¨ Rust å¼åç½ç»è½¯ä»¶ãä»ä½¿ç¨å¥æ¥å­çå®¢æ·ç«¯-æå¡å¨ç½ç»å° IPv4/v6ãDNSãTCPãUDPï¼æ¨è¿å°äºè§£ä½¿ç¨ serde åºåååååºååæ°æ®ãè¿æ¬ä¹¦å±ç¤ºäºå¦ä½éè¿ HTTP ä¸ REST æå¡å¨è¿è¡éä¿¡ãæ¬ä¹¦çæåä¸é¨åè®¨è®ºäºä½¿ç¨ Tokio å æ è¿è¡å¼æ­¥ç½ç»ç¼ç¨ãé´äºå®å¨å¯¹äºç°ä»£ç³»ç»çéè¦æ§ï¼æ¨å°çå° Rust å¦ä½æ¯æå¸¸è§çåè¯­ï¼ä¾å¦ TLS åå¬é¥å å¯ã
  
- [ãRust Programming by Exampleã](https://kr1lib.org/book/5669466/ef3a67) 
  
ä»ä»ç» Rust å¼å§ï¼æ¨å°å­¦ä¹ åºæ¬æ¹é¢ï¼ä¾å¦å¶è¯­æ³ãæ°æ®ç±»åãå½æ°ãæ³åãæ§å¶æµç­ãå¨æ­¤ä¹åï¼æ¨å°ç´æ¥å¼å§æå»ºæ¨çç¬¬ä¸ä¸ªé¡¹ç®ï¼ä¿ç½æ¯æ¹åæ¸¸æãæ¥ä¸æ¥ï¼æ¨å°ä½¿ç¨ Tokioï¼å¯æ©å±ä¸é«æçå¼æ­¥ IO Rust åºï¼æå»ºå¾å½¢é³ä¹æ­æ¾å¨å¹¶ä½¿ç¨å¿«éãå¯é çç½ç»è½¯ä»¶ã

å¨æ¬ä¹¦çè¿ç¨ä¸­ï¼æ¨å°æ¢ç´¢ Rust ç¼ç¨çåç§ç¹æ§ï¼åæ¬å®ç SDL ç¹æ§ãäºä»¶å¾ªç¯ãæä»¶ I/O åèåç GTK+ å°é¨ä»¶å·¥å·åãéè¿è¿äºé¡¹ç®ï¼æ¨å°çå° Rust å¨å¹¶åæ¹é¢çè¡¨ç°ââåæ¬å¹¶è¡æ§ãå¯é æ§ãæ¹è¿çæ§è½ãæ³åãå®åçº¿ç¨å®å¨ãæä»¬è¿å°ä»ç» Rust çä¸äºå¼æ­¥åååºå¼ç¼ç¨æ¹é¢ã
  
- [ãRust Quick Start Guideã](https://kr1lib.org/book/11689628/cf06fb)
  
çæä½¿ç¨æµè¡çæ°ç³»ç»ç¼ç¨è¯­è¨ç¼åç¨åºï¼è¿äºè¯­è¨å°ä½çº§è¯­è¨çå¼ºå¤§æ§è½ä¸å¤çº¿ç¨ä»£ç ä¸­ççº¿ç¨å®å¨ç­é«çº§åè½ç»åå¨ä¸èµ·ã
  
- [ãRust in Action [MEAP]ã](https://kr1lib.org/book/11235796/a7ef40)  
  
Rust in Action æ¯ä¸æ¬é¢åæ³è¦æ¢ç´¢ Rust ç¼ç¨è¯­è¨ä¸ççä¸­çº§ç¨åºåçä¹¦ãå®éç¨äºå¯è½å·²ç»ç¨å°½ç½ç»ä¸çåè´¹èµæä½ä»æ³äºè§£æ´å¤ä¿¡æ¯çäººãå®ä¸ Rust ç¼ç¨çå¶ä»ææä¸åï¼å ä¸ºå®è¿ææ¨æå³ç³»ç»ç¼ç¨çç¥è¯ãæ¨å°è½å¤æ´å¤å°äºè§£ CPU çå·¥ä½åçãè®¡ç®æºå¦ä½è®¡æ¶ãæéæ¯ä»ä¹ä»¥åæ¨çç½å¡åé®çå¦ä½åè¯ CPU å®ä»¬å·²åå¤å¥½è¯»åè¾å¥ã

ä»ç³»ç»ç¼ç¨ä¹¦ç±çè§åº¦æ¥çï¼å®å®éä¸ä¹æ¯ç¬ä¸æ äºç - å ä¸ºå ä¹æ¯ä¸ªç¤ºä¾é½éç¨äº Windowsï¼å¦æä½ æ¯é£ç§åæ¬¢å®éä¾å­çå­¦ä¹ èï¼ä½ ä¼åæ¬¢éè¯»è¿æ¬ä¹¦ã
  
- [ãA Gentle Introduction to Rustã](https://stevedonovan.github.io/rust-gentle-intro/)  
  
Rust æ¯ä¸ç§éæåå¼ºç±»åçç³»ç»ç¼ç¨è¯­è¨ãéææå³çææç±»åå¨ç¼è¯æ¶é½æ¯å·²ç¥çï¼å¼ºçæå³çè¿äºç±»åæ¨å¨ä½¿ç¼åä¸æ­£ç¡®çç¨åºåå¾æ´å å°é¾ãä¸ä¸ªæåçç¼è¯æå³çä½ å¯ä»¥æ¯ä½¿ç¨å C è¿æ ·ççä»è¯­è¨æ´å¥½å°ä¿è¯æ­£ç¡®æ§ãç³»ç»æå³ççææå¥½çæºå¨ä»£ç ï¼å¹¶å®å¨æ§å¶åå­ä½¿ç¨ãå æ­¤ï¼å¶ç¨ééå¸¸æ ¸å¿ï¼æä½ç³»ç»ãè®¾å¤é©±å¨ç¨åºåçè³å¯è½æ²¡ææä½ç³»ç»çåµå¥å¼ç³»ç»ãç¶èï¼å®å®éä¸ä¹æ¯ä¸ç§éå¸¸ä»¤äººæå¿«çè¯­è¨ï¼å¯ä»¥ç¨æ¥ç¼åæ®éçåºç¨ç¨åºä»£ç ã

ä¸ C å C++ çæå¤§åºå«å¨äº Rust é»è®¤æ¯å®å¨çï¼æ£æ¥ææåå­è®¿é®ãæå¤æååå­æ¯ä¸å¯è½çã
  
- [ãPractical Machine Learning with Rust: Creating Intelligent Applications in Rustã](https://kr1lib.org/book/5304256/0ff807)  
  
Rust ä¸­çæºå¨å­¦ä¹ å·²ç»è¢«ç¤¾åºå¿½è§äºå¾é¿ä¸æ®µæ¶é´ãç±äºå®å®ä¸­æ£å¸çè®¸å¤ä¸åçæ¿æ¡ç®±ï¼è¿æ¬ä¹¦è¯å¾ç»ä¸ææçä¿¡æ¯åç¨æ³ï¼å¹¶å¨æç§ç¨åº¦ä¸å¨æç¤¾åºéåè¡å¨ãæ°æ®æ¯æ°çåæ²¿é¢åï¼è Rust å¿é¡»æä¸ºå¶ä¸­çä¸é¨åã

éè¯»äºä½¿ç¨ Rust çå®ç¨æºå¨å­¦ä¹ ä¹åï¼æ¨å°å¯¹ä½¿ç¨ Rust åå»ºé«è®¡ç®åºæä¸ä¸ªæ·±å¥çäºè§£ãææ¡äºè¿ç§ç¥å¥è¯­è¨çç¥è¯ï¼æ¨å°è½å¤åå»ºæ§è½æ´é«ãåå­å®å¨ä¸èµæºå ç¨æ´å°çåºç¨ç¨åºã
  
- [ãRust Web Developmentã](https://kr1lib.org/book/11729741/a127f0)  

Rust Web Development æ¯ä½¿ç¨ Rust æå»ºåºäºæå¡å¨ç Web åºç¨ç¨åºçå®è·µæåãå¦ææ¨ä½¿ç¨ JavaãC# æ PHP æå»ºäº Web æå¡å¨ï¼æ¨ä¼ç«å³ç±ä¸ Rust æä¾çæ§è½åå¼åä½éªãæ¬ä¹¦åæ¨å±ç¤ºäºå¦ä½ä½¿ç¨çº¯ Rust ä»¥åéè¦ç Rust åºï¼ä¾å¦ç¨äºå¼æ­¥è¿è¡æ¶ç tokioãç¨äº Web æå¡å¨å API ç warp ä»¥åè¿è¡å¤é¨ HTTP è¯·æ±ç reqwest ç­ï¼é«æå·¥ä½ã

æ¨å¯ä»¥å°è¿æ¬ä¹¦äº¤ç»æ°èç¨çå¼åäººåï¼å¹¶è®©ä»ä»¬ä½¿ç¨è¿æ¬ä¹¦ãå®åå«éå¸¸å®ç¨çç¤ºä¾åæ¨¡å¼ï¼å¹¶ä¸ºæªæ¥æ¢ç´¢è¯¥ä¸»é¢å¥ å®äºåå®çåºç¡ã
  
**è¿é¶ä¹¦ç±**
 
- [ãThe Rustonomiconã](https://doc.rust-lang.org/nightly/nomicon/)
  
æ¬ä¹¦æ·±å¥æ¢è®¨äºç¼åæ­£ç¡®çä¸å®å¨ Rust ç¨åºæéçææå¯æç»èãç±äºè¿ä¸ªé®é¢çæ§è´¨ï¼å®å¯è½ä¼å¯¼è´éæ¾åºæ æ³è¨å»çææï¼å°ä½ çå¿çµç²ç¢æåäº¿ä¸ªæ éå°çç»æç¢çã

å¦ææ¨å¸æç¼å Rust ç¨åºçèä¸çæ¶¯é¿ä¹èå¿«ä¹ï¼é£ä¹ç°å¨æ¨åºè¯¥åè¿å¤´æ¥å¿è®°æ¨æ¾ç»çè¿è¿æ¬ä¹¦ãè¿ä¸æ¯å¿è¦çãä½æ¯ï¼å¦ææ¨æç®ç¼åä¸å®å¨çä»£ç ââæèåªæ¯æ³æ·±å¥äºè§£è¯­è¨çæ¬è´¨ââè¿æ¬ä¹¦åå«äºå®è´µçä¿¡æ¯ã  
  
- [ãProgramming Rustã](https://1lib.limited/book/3400043/791885) 
  
è¿æ¬å®ç¨çä¹¦åç³»ç»ç¨åºåä»ç»äº Rustï¼ä¸ç§æ°çåæ²¿è¯­è¨ãæ¨å°äºè§£ Rust å¦ä½æä¾éæéªè¯çåå­å®å¨åä½çº§æ§å¶çç½è§ä¸æä»·å¼çç»åââæ³è±¡ä¸ä¸ C++ï¼ä½æ²¡ææ¬ç©ºæéãç©ºæéåæ¶å¼ç¨ãæ³æ¼æç¼å²åºæº¢åºã  
  
- [ãRust Essentials - Second Editionã](https://1lib.limited/book/3427870/81d715)  
  
æ¬ä¹¦é¦åè®ºè¯äº Rust å¨å½ä»ç¼ç¨è¯­è¨é¢åçç¬ç¹å°ä½ãå®è£ Rust å¹¶å­¦ä¹ å¦ä½ä½¿ç¨å®çåç®¡çå¨ Cargoãéæ­¥ä»ç»åç§æ¦å¿µï¼åéãç±»åãå½æ°åæ§å¶ç»æï¼ä»¥æä¸åºç¡ãç¶åæ¢ç´¢æ´å¤ç»æåæ°æ®ï¼ä¾å¦å­ç¬¦ä¸²ãæ°ç»åæä¸¾ï¼å¹¶äºè§£æ¨¡å¼å¹éçå·¥ä½åçã

å¨è¿ä¸åä¸­ï¼æ¬ä¹¦å¼ºè°äº Rust ç¼è¯å¨ç¨æ¥çæå®å¨ä»£ç çç¬ç¹æ¨çæ¹å¼ãæ¥ä¸æ¥çç Rust ç¹å®çéè¯¯å¤çæ¹å¼ï¼ä»¥åç¹å¾å¨ Rust ä»£ç ä¸­çæ´ä½éè¦æ§ãå¨æä»¬æ¢ç´¢åç§æéç±»åæ¶ï¼å°æ·±å¥æ¢è®¨åå­å®å¨çæ¯æ±ãæ¥ä¸æ¥ï¼ççå®å¦ä½ç®åä»£ç çæï¼ä»¥åå¦ä½ä½¿ç¨æ¨¡ååæ¿æ¡ç®±ç»åæ´å¤§çé¡¹ç®ãæåï¼äºè§£æä»¬å¦ä½å¨ Rust ä¸­ç¼åå®å¨çå¹¶åä»£ç å¹¶ä¸ C ç¨åºæ¥å£ï¼äºè§£ Rust çæç³»ç»ï¼å¹¶æ¢ç´¢æ ååºçä½¿ç¨ã  
  
- [ãHands-On Concurrency with Rustã](https://1lib.limited/book/11689707/4154e1)  
  
æ¬ä¹¦å°æä½ å¦ä½å¨ç°ä»£æºå¨ä¸ç®¡çç¨åºæ§è½ï¼å¹¶å¨ Rust ä¸­æå»ºå¿«éãåå­å®å¨åå¹¶åçè½¯ä»¶ãå®ä» Rust çåºç¡å¼å§ï¼è®¨è®ºæºå¨æ¶ææ¦å¿µãæ¨å°äºè§£å¦ä½ç³»ç»å°è¡¡éåæ¹è¿ Rust ä»£ç çæ§è½ï¼ä»¥åå¦ä½èªä¿¡å°ç¼åéåãæ¨å°äºè§£åºç¨äºçº¿ç¨ç Sync å Send ç¹æ§ï¼å¹¶ä½¿ç¨éãåå­åè¯­ãæ°æ®å¹¶è¡ç­æ¥åè°çº¿ç¨æ§è¡ã

æ¬ä¹¦å°åæ¨å±ç¤ºå¦ä½å¨ C++ ä»£ç ä¸­ææå°åµå¥ Rustï¼å¹¶æ¢ç´¢ç¨äºå¤çº¿ç¨åºç¨ç¨åºçåç§ crate çåè½ãå®æ·±å¥æ¢è®¨äºå®ç°ãæ¨å°äºè§£äºæ¥éçå·¥ä½åçå¹¶èªè¡æå»ºå¤ä¸ªäºæ¥éãæ¨å°ææ¡çæç³»ç»ä¸­å­å¨çå®å¨ä¸åçæ¹æ³æ¥æå»ºåç®¡çå¤§è§æ¨¡ç³»ç»ã
  
- [ãHands-On Functional Programming in Rustã](https://1lib.limited/book/11689735/4d162e)
  
å½æ°å¼ç¼ç¨åè®¸å¼åäººåå°ç¨åºååä¸ºæ´å°çãå¯éç¨çç»ä»¶ï¼ä»æ´ä½ä¸ç®åè½¯ä»¶çåå»ºãæµè¯åç»´æ¤ãç»å Rust çå¼ºå¤§åè½ï¼æ¨å¯ä»¥å¼åæ»¡è¶³ç°ä»£è½¯ä»¶éæ±çå¼ºå¤§ä¸å¯æ©å±çåºç¨ç¨åºãæ¬ä¹¦å°å¸®å©æ¨åç°å¯ç¨äºä»¥åè½æ¹å¼æå»ºè½¯ä»¶çææ Rust åè½ã

æä»¬é¦åå¯¹éå¯¹ä¸åé®é¢åæ¨¡å¼çå½æ°å¼æ¹æ³åé¢åå¯¹è±¡æ¹æ³è¿è¡ç®è¦æ¯è¾ãç¶åæä»¬å¿«éæ¥çæ§å¶æµçæ¨¡å¼ãæ°æ®ä»¥åè¿äºå½æ°å¼ç¼ç¨ç¬æçæ½è±¡ãä¸ä¸é¨åä»ç»å¦ä½å¨ Rust ä¸­åå»ºåè½æ§åºç¨ç¨åºï¼è¿è®¨è®ºäº Rust ç¬æçå¯åæ§åæææãæ¥ä¸æ¥æ£æ¥çº¯å½æ°ï¼æ¨å°ææ¡é­åãå®ä»¬çåç§ç±»ååæ¯éåãæä»¬è¿éè¿åè½è®¾è®¡åååä½¿ç¨å®çåç¼ç¨æ¥å®ç°å¹¶åãæåï¼æä»¬ççè°è¯åä¼åçæä½³å®è·µã

è¯»å®æ¬ä¹¦ï¼æ¨å°çæå½æ°å¼ç¼ç¨æ¹æ³ï¼å¹¶è½å¤å¨æ¥å¸¸å·¥ä½ä¸­ä½¿ç¨è¿äºææ¯ã  
  
- [ãRust High Performanceã](https://1lib.limited/book/11000538/3e9291)
  
ææ¶ï¼å¾é¾ä» Rust ä¸­è·å¾æä½³æ§è½ãè¿æ¬ä¹¦æä½ å°ä½ ç Rust ä»£ç çéåº¦ä¼åå° C/C++ ç­è¯­è¨çæ°´å¹³ãæ¨å°äºè§£å¹¶ä¿®å¤å¸¸è§çé·é±ï¼äºè§£å¦ä½éè¿ä½¿ç¨åç¼ç¨æ¥æé«çäº§åï¼å¹¶éè¿å®å¨è½»æ¾å°å¹¶åæ§è¡é¨åä»£ç æ¥å éä»£ç ãæ¨å°ææ¡è¿é¨è¯­è¨çç¹æ§ï¼è¿å°ä½¿æ¨è±é¢èåºï¼å¹¶ä½¿ç¨å®ä»¬æ¥çæ­£æé«ç®æ³çæç

æ¬ä¹¦ä»¥ä¸ä¸ªæ¸©åçä»ç»å¼å§ï¼ä»¥å¸®å©æ¨è¯å« Rust ç¼ç¨æ¶çç¶é¢ãæä»¬éç¹ä»ç»äºå¸¸è§çæ§è½ç¼ºé·ï¼ä»¥ååæ©åç°åè§£å³è¿äºé®é¢çç­ç¥ãæä»¬ç»§ç»­ææ¡ Rust çç±»åç³»ç»ï¼è¿å°ä½¿æä»¬è½å¤å¨ç¼è¯æ¶å¨æ§è½åå®å¨æ§æ¹é¢è¿è¡ä»¤äººå°è±¡æ·±å»çä¼åãç¶åï¼æ¨å°å­¦ä¹ å¦ä½å¨ Rust ä¸­ææå°ç®¡çåå­ï¼ææ¡åç¨æ£æ¥å¨ãæä»¬ç»§ç»­æµéæ§è½ï¼æ¨å°çå°è¿å¦ä½å½±åæ¨ç¼åä»£ç çæ¹å¼ãç»§ç»­åè¿ï¼æ¨å°å¨ Rust ä¸­æ§è¡åç¼ç¨ï¼ä»¥æé«ä»£ç çæ§è½åçäº§åãæ¨æç»å°å­¦ä¹  Rust ä¸­çå¹¶è¡ç¼ç¨ï¼å®éè¿ä½¿ç¨å¤çº¿ç¨åå¼æ­¥ç¼ç¨å®ç°é«æåæ´å¿«çæ§è¡ã
  
- [ãZero To Production In Rustã](https://zero2prod.com/) 
  
å¦ææ¨æ³å­¦ä¹ å¦ä½ä½¿ç¨ Rust è¿è¡åç«¯å¼åï¼è¿éå°±æ¯æ¨çæä½³éæ©ã

Rust çéç¨çè¾¾å°äºåå²æé«æ°´å¹³ï¼è¶æ¥è¶å¤çå¬å¸æ­£å¨å°è¯åæèã<br>
å¦ææ¨å¯¹ä½¿ç¨ Rust æå»º API æå´è¶£ï¼é¶å°çäº§æ¯æ¨ Rust ä¹æççæ³èµ·ç¹ã<br>
æ¨å°è¾¹åè¾¹å­¦ï¼æä»¬å°ä»å¤´å¼å§ï¼ä¸æ­¥ä¸æ­¥å°æå»ºä¸ä¸ªåè½é½å¨ççµå­é®ä»¶éè®¯åç«¯ APIã<br>

æ¨å°å­¦ä¹ ï¼

1ãå¯¼èªåå©ç¨ Rust ç crates çæç³»ç»<br>
2ãæå»ºæ¨çåºç¨ç¨åºä»¥ä½¿å¶æ¨¡åååå¯æ©å±<br>
3ãç¼åæµè¯ï¼ä»åä¸ªååå°æççéææµè¯<br>
4ãä½¿ç¨ç±»åç³»ç»ä¸ºæ¨çåå»ºæ¨¡ä»¥å¼ºå¶æ§è¡ä¸åé<br>
5ãæ¶éæ¥å¿ãè·è¸ªåææ ä»¥è§å¯åºç¨ç¨åºçç¶æ<br>
6ãä¸ºæ¨ç Rust é¡¹ç®è®¾ç½®ä¸ä¸ªå¼ºå¤§çæç»­éæåæç»­é¨ç½²ç®¡é<br>
  
- [ãProgramming WebAssembly with Rustã](https://1lib.limited/book/5001228/7b21a9)  
  
WebAssembly ä¸ä»ä»æ¯ä¸é¡¹é©å½æ§çæ°ææ¯ãå®æ­£å¨éå¡æä»¬ä¸º Web åå¶ä»é¢åæå»ºåºç¨ç¨åºçæ¹å¼ãå¨ ActiveX å Flash ç­ææ¯å¤±è´¥çå°æ¹ï¼æ¨ç°å¨å¯ä»¥ä½¿ç¨æ¨åæ¬¢çä»»ä½è¯­è¨ç¼åä»£ç å¹¶ç¼è¯ä¸º WebAssemblyï¼ä»¥ä¾¿å¨æµè§å¨ãç§»å¨è®¾å¤ãåµå¥å¼è®¾å¤ç­ä¸­è¿è¡çå¿«éãç±»åå®å¨çä»£ç ãå° WebAssembly çä¾¿æºãé«æ§è½æ¨¡åä¸ Rust çå®å¨æ§åå¼ºå¤§åè½ç¸ç»åï¼æ¯ä¸ä¸ªå®ç¾çå¼åç»åã

äºè§£ WebAssembly çå æ æºå¨æ¶æå¦ä½å·¥ä½ï¼å®è£ä½çº§ wasm å·¥å·ï¼å¹¶åç°ç¼ååå§åºå¼ä»£ç çé»æèºæ¯ãå¨æ­¤åºç¡ä¸æå»ºå¹¶å­¦ä¹ å¦ä½éè¿å®ç°è·³æ£æ¸¸æçé»è¾ä» Rust ç¼è¯ WebAssembly æ¨¡åãå¨ Rust ä¸­åå»º wasm æ¨¡åï¼ä»¥å¤ç§å¼äººæ³¨ç®çæ¹å¼ä¸ JavaScript è¿è¡äºæä½ãå°æ¨çæ°æè½åºç¨äºéç½ç»ä¸»æºçä¸çï¼å¹¶åå»ºä»å¨ Raspberry Pi ä¸è¿è¡çæ§å¶ç§æç³»ç»çåºç¨ç¨åºå°åè½é½å¨çå¨çº¿å¤äººæ¸¸æå¼æï¼å¼åäººåå¯ä»¥ä¸ä¼ ä»ä»¬èªå·±çç«æåºç»å® WebAssembly æææ¨¡å.

ç«å³å¼å§ä½¿ç¨ WebAssemblyï¼å¹¶æ¹åæ¨å¯¹ Web ççæ³ã  
  
- [ãStep Ahead with Rust: Systems Programming in Rustã](https://www.armstrong-publications.com/product/step-ahead-with-rust-super-combo/)  
  
ä»åºæ¬çç¼ç¨æ¨¡å¼å°æ·±å¥äºè§£è¯¥è¯­è¨ï¼Step Ahead with Rust æ¨å¨å¸®å©æ¨ä»ç¼åç¨åºå°ä½¿ç¨ Rust æå»ºè½¯ä»¶ãæ¬ä¹¦å°åæ¨å±ç¤º Rust è¯­è¨æéè¦çç¹æ§ï¼åæ¬è´§ç©ãç±»åç³»ç»ãè¿­ä»£å¨ç­ãè¯»å®æ¬ä¹¦ï¼æ¨åºè¯¥ä¼çææ´å¤åå®¹ï¼å¹¶åå¤å¥½å¤çå¶ä½çé«çº§ä¸»é¢ã

å¨æ¨éè¯»æ¬ä¹¦çè¿ç¨ä¸­ï¼æä»¬å»ºè®®æ¨è±æ¶é´å°è¯ä¸ä¸ä¹¦é¡µä¸­æåç°çåå®¹ãè¿æ¬ä¹¦é½æ¯å³äº Rust çå®éåºç¨ï¼æä»¥å¨å®è·µä¸­åºç¨å®æ¯å¼å¾æå¾çãæ¬ä¹¦æ¶µçï¼è´§ç©ãRust ç±»åç³»ç»ãè¿­ä»£å¨ãå®ãæææãåç¨åçå½å¨æãä¸å®å¨æ¨¡å¼ãå¹¶åãA Step Ahead with Rust è¯»èåºè¯¥æ¯ä¸ä½ç»éªä¸°å¯çå¼åäººåï¼å¸ææé«ä»ä»¬ç Rust å¼åæè½ã  
  
- [ãCreative Projects for Rust Programmersã](https://1lib.limited/book/5639719/c52aca)  
  
äºè§£ Rust ç¼ç¨è¯­è¨çææ°ç¹æ§ãæç¨çåºåæ¡æ¶çå®ç¨æåï¼å°å¸®å©æ¨è®¾è®¡åå¼åæè¶£çé¡¹ç®

å­¦ä¹ ï¼

1ãè®¿é® TOMLãJSON å XML æä»¶ä»¥å SQLiteãPostgreSQL å Redis æ°æ®åº<br>
2ãä½¿ç¨ JSON ææè´è½½å¼å RESTful Web æå¡<br>
3ãä½¿ç¨ HTML æ¨¡æ¿å JavaScript åå»º Web åºç¨ç¨åºï¼ä½¿ç¨ WebAssembly åå»ºåç«¯ Web åºç¨ç¨åºæ Web æ¸¸æ<br>
4ãæå»ºæ¡é¢ 2D æ¸¸æ<br>
5ãä¸ºç¼ç¨è¯­è¨å¼åè§£éå¨åç¼è¯å¨<br>
6ãåå»ºæºå¨è¯­è¨æ¨¡æå¨<br>
7ãä½¿ç¨å¯å è½½æ¨¡åæ©å± Linux åæ ¸<br>
  
# ð å¤§çæç« 
  
- [çè§£ Rust ççå½å¨æ](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E7%90%86%E8%A7%A3%20Rust%20%E7%9A%84%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F.md)
- [é«å¾·ææ¯ | åºäºRustçAndroid Nativeåå­åææ¹æ¡](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/%E5%9F%BA%E4%BA%8ERust%E7%9A%84Android%20Native%E5%86%85%E5%AD%98%E5%88%86%E6%9E%90%E6%96%B9%E6%A1%88.md)
- [Rust ä¸ C++ï¼æ·±å¥çè¯­è¨æ¯è¾](https://github.com/0voice/Understanding_in_Rust/blob/main/%E6%96%87%E7%AB%A0/Rust%20%E4%B8%8E%20C%2B%2B%EF%BC%9A%E6%B7%B1%E5%85%A5%E7%9A%84%E8%AF%AD%E8%A8%80%E6%AF%94%E8%BE%83.md)
  
# ð° å®æ¹ææ¡£
  
- [æ ååºAPIææ¡£](https://doc.rust-lang.org/std/)
- [Rust Reference](https://doc.rust-lang.org/reference/index.html): Rust reference ææ¡£ï¼æä¸­æç¿»è¯çæ¬ [Rustè¯­è¨è§è](https://rustlang-cn.org/office/rust/reference/) æ­£å¨ç¿»è¯è¿ç¨ä¸­
- [Rustç¼è¯éè¯¯ç´¢å¼](https://doc.rust-lang.org/error-index.html)ï¼åçç¼è¯éè¯¯æ¶ï¼å¯ä»¥éè¿ç´¢å¼æ¾å°å·ä½éè¯¯è§£é
- [rustdocææ¡£](https://doc.rust-lang.org/rustdoc/): `restdoc`å·¥å·çä½¿ç¨ææ¡£
- [Rustonomicon](https://doc.rust-lang.org/reference/): rustçåèææ¡£ãä½æ¯ç®åå¹¶ä¸å®æ´ï¼å¯è½æéæ¼åéè¯¯
- [Unstable Book](https://doc.rust-lang.org/unstable-book/): ç¨äºå°ä¸ç¨³å®ç¹æ§çææ¡£
- [Rustonomicon](https://doc.rust-lang.org/nomicon/): unsafe rustçé»æèºæ¯ï¼æä¸­æç¿»è¯çæ¬ [Rusté«çº§ç¼ç¨](https://rustlang-cn.org/office/rust/advrust/)
- [The Cargo Book](https://doc.rust-lang.org/cargo/index.html): cargoä½¿ç¨ä»ç»ï¼æä¸­æç¿»è¯çæ¬ [Cargoæç¨](https://rustlang-cn.org/office/rust/cargo/) æ­£å¨è¿è¡ä¸­
- [Rust Edition Guide](https://doc.rust-lang.org/nightly/edition-guide/introduction.html): Rust çæ¬æåï¼ä¼ é Rust ä¸åçæ¬ä¹é´å¤§çåæ´ä¿¡æ¯
- [Command line apps in Rust](https://rust-lang-nursery.github.io/cli-wg/#command-line-apps-in-rust): å¨Rustä¸­ç¼åå½ä»¤è¡ç¨åº
  
# â æè´§éº
  
- Rust æå¤§ä¸­æç¤¾åºè®ºåï¼https://rustcc.cn/
- å°ä¼ä¸­æç¤¾åºçç¿»è¯èµæ/è®ºåï¼https://learnku.com/rust
- Rustå¨çº¿ç¼è¾å¨: https://play.rust-lang.org/
- 2021 å¹´å»åªå­¦ Rustï¼https://loige.co/where-to-go-to-learn-rust-in-2021/
- Rust Cheat Sheetï¼Rustè¯­æ³å¤å¿åï¼ï¼https://cheats.rs/
- Rust ä¸­æä¹¦æ¶ä¸èµè®¯ï¼https://budshome.com/ | https://blog.budshome.com/
- ç®è¦èåºç¡ç Rust ç¥è¯ï¼éåå¨ Rust Book é¶æ®µå½ä½è¡¥åææï¼ï¼https://learning-rust.github.io/
- å¾®è½¯åå¸ç Rust æ°ææç¨ï¼https://docs.microsoft.com/en-us/learn/paths/rust-first-steps/
- Rust-leetcodeså·é¢ï¼https://stevenbai.top/rust-leetcode/
- Rust by Example éè¿ä¾å­å­¦ Rustï¼https://doc.rust-lang.org/rust-by-example/index.html
- çµå­ä¹¦ä¸è½½ ï¼https://jp1lib.org/s/Rust
- Rustçº¿ä¸å¨çä¼è®®ï¼
  - RustConf: https://rustconf.com/
  - Rust Belt Rust: https://rust-belt-rust.com/
  - RustFest: https://blog.rustfest.eu/
  - Rust Latam: https://rustcon.asia/
  - RustCon Asia: https://rustcon.asia/
  
# ð½ è§é¢
  
Rust éªè¯ç è®¨ä¼ 2021 | 
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
[Prusti â Deductive Verification for Rust](https://www.aliyundrive.com/s/eph1UzJugSt)|
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
  
  

# ð å¼æºæ¡æ¶
  
## å¼å¾æ°æå³æ³¨çRusté¡¹ç®

- [mini redis](https://github.com/tokio-rs/mini-redis) - ä¸å®æ´çRediså®¢æ·ç«¯åæå¡å¨å®ç°ä½¿ç¨Tokio -ä»ä¸ºå­¦ä¹ ç®ç
- [async-graphql](https://github.com/sunli829/async-graphql) - ä¸ä¸ªå¨Rustä¸­å®ç°çGraphQLæå¡å¨åº
  
## åºç¨ç¨åº

- [alacritty](https://github.com/alacritty/alacritty) â è·¨å¹³å°ãGPU å¢å¼ºçç»ç«¯æ¨¡æå¨
- [AnderEnder/s3find-rs](https://github.com/AnderEnder/s3find-rs) â ç¨äºéå Amazon S3 å±æ¬¡ç»æçå½ä»¤è¡å®ç¨ç¨åºï¼ç±»ä¼¼äº Amazon S3 ç find
- [andschwa/rust-genetic-algorithm](https://github.com/andschwa/rust-genetic-algorithm) â ä¸ç§ç¨äºå­¦æ¯åºåé®é¢çéä¼ ç®æ³
- [asm-cli-rust](https://github.com/cch123/asm-cli-rust) â ä¸ä¸ªç¨ Rust ç¼åçäº¤äºå¼ç¨åºéå¤å£³.
- [ballista](https://github.com/ballista-compute/ballista) â ä½¿ç¨ RustãApache Arrow å Kubernetes çåå¸å¼è®¡ç®å¹³å°ç PoCï¼
- [cloudflare/boringtun](https://github.com/cloudflare/boringtun) â ç¨æ·ç©ºé´ WireGuard VPN å®ç°
- [darrint/device-blocker](https://github.com/darrint/device-blocker) â éè¿é»æ­¢å®¶åº­ Wifi è·¯ç±å¨ä¸çäºèç½è®¿é®æ¥éå¶å¿ç«¥åç§ç§»å¨è®¾å¤çå±å¹æ¶é´.
- [denoland/deno](https://github.com/denoland/deno) â ä½¿ç¨ V8ãRust å Tokio æå»ºçå®å¨ JavaScript/TypeScript è¿è¡æ¶
- [dlecan/generic-dns-update](https://github.com/dlecan/generic-dns-update) â ä½¿ç¨æ¨ç IP å°åæ´æ° DNS åºåæä»¶çå·¥å·
- [Factotum](https://github.com/snowplow/factotum) â [A system to programmatically run data pipelines](https://snowplowanalytics.com/blog/2016/04/09/introducing-factotum-data-pipeline-runner/) 
- [fcsonline/drill](https://github.com/fcsonline/drill) â å Ansible è¯­æ³å¯åç HTTP è´è½½æµè¯åºç¨ç¨åº
- [Fractalide](https://github.com/fractalide/fractalide) â ç®åç Rust å¾®æå¡
- [habitat](https://community.chef.io/tools/chef-habitat) â ä¸ä¸ªå·¥å· [Chef](https://www.chef.io/) æå»ºãé¨ç½²åç®¡çåºç¨ç¨åº.
- [Herd](https://github.com/imjacobclark/Herd) â ä¸ä¸ªå®éªæ§ç HTTP è´è½½æµè¯åºç¨ç¨åº
- [intecture/api](https://github.com/intecture/api) â API é©±å¨çæå¡å¨ç®¡çåéç½®å·¥å·
- [ivanceras/diwata](https://github.com/ivanceras/diwata) â postgresql çæ°æ®åºç®¡çå·¥å·
- [jedisct1/flowgger](https://github.com/awslabs/flowgger) â å¿«éãç®ååè½»éçº§çæ°æ®æ¶éå¨
- [kbknapp/docli](https://github.com/kbknapp/docli-rs) â ç¨äºç®¡ç DigitalOcean åºç¡è®¾æ½çå½ä»¤è¡å®ç¨ç¨åº 
- [kytan](https://github.com/changlan/kytan) â é«æ§è½ç¹å¯¹ç¹ VPN
- [limonite](https://crates.io/crates/limonite) â éæåå®¢ / ç½ç«çæå¨ 
- [linkerd/linkerd2-proxy](https://github.com/linkerd/linkerd2-proxy) â Kubernetes çè¶è½»æå¡ç½æ ¼.
- [MaidSafe](https://maidsafe.net/) â ä¸ä¸ªå»ä¸­å¿åçå¹³å°.
- [mdBook](https://crates.io/crates/mdbook) â ä» Markdown æä»¶åå»ºä¹¦ç±çå½ä»¤è¡å®ç¨ç¨åº 
- [nicohman/eidolon](https://github.com/nicohman/eidolon) â éç¨äº linux å macosx çæ  Steam å drm æ¸¸ææ³¨åè¡¨åå¯å¨å¨
- [notty](https://github.com/withoutboats/notty) â ä¸ç§æ°åç»ç«¯
- [Pijul](https://pijul.org/) â åºäºè¡¥ä¸çåå¸å¼çæ¬æ§å¶ç³»ç»
- [rsign](https://crates.io/crates/rsign) â ä¸ä¸ªç®åçå½ä»¤è¡å·¥å·ï¼ç¨äºçæ / ç­¾ç½² / éªè¯æ¨å¨ä¸ Minisign å¼å®¹çæ°å­ç­¾å 
- [Rudr](https://github.com/oam-dev/rudr) â Kubernetes å®ç° [Open Application Model](https://oam.dev/) è§æ ¼
- [rx](https://github.com/cloudhead/rx) â å Vi å¯åçç°ä»£åç´ èºæ¯ç¼è¾å¨
- [Sandstorm Collections App](https://github.com/sandstorm-io/collections-app)
- [Servo](https://github.com/servo/servo) â åå Web æµè§å¨å¼æ
- [tiny](https://github.com/osa1/tiny) â ç»ç«¯ IRC å®¢æ·ç«¯
- [trust-dns](https://crates.io/crates/trust-dns) â DNS æå¡å¨
- [updns](https://github.com/wyhaya/updns) â DNS ä»£çå·¥å·
- [Weld](https://github.com/serayuzgur/weld) â å¨å REST API çæå¨ 
- [wezterm](https://github.com/wez/wezterm) â ä¸ä¸ªgpuå éçè·¨å¹³å°ç»ç«¯æ¨¡æå¨åå¤è·¯å¤ç¨å¨
  
### é³é¢åé³ä¹ææ¯

- [enginesound](https://github.com/DasEtwas/enginesound) â ç¨äºæç¨åºçæåé¼çå¼æå£°é³ç GUI åå½ä»¤è¡åºç¨ç¨åº. å·ææ·±åº¦éç½®ãå¯åéæ ·çåé¢çåæçªå£.
- [indiscipline/zrtstr](https://github.com/indiscipline/zrtstr) â ç¨äºæ£æ¥ç«ä½å£° wav æä»¶æ¯å¦ä¸ºä»¿ç«ä½å£°ï¼å³å·æç¸åééï¼å¹¶å°æ­¤ç±»æä»¶è½¬æ¢ä¸ºåå£°éçå½ä»¤è¡å®ç¨ç¨åº.
- [Lyriek](https://github.com/bartwillems/lyriek) â ä¸ä¸ªå¤çº¿ç¨ GTK 3 åºç¨ç¨åºï¼ç¨äºè·åå½åæ­æ¾æ­æ²çæ­è¯.
- [Phate6660/musinfo](https://github.com/Phate6660/musinfo) â ä» mpd æ¥è¯¢é³ä¹ä¿¡æ¯å¹¶å°å¶æ¾ç¤ºå¨éç¥ä¸­çç¨åº.
- [Phate6660/rsmpc](https://github.com/Phate6660/rsmpc) â mpc çå®ç°ï¼ä½ä¸æ¯ç´æ¥å®ç°ï¼å ä¸ºä¼æä¸äºå·®å¼.
- [Phate6660/rsmpc](https://github.com/Phate6660/rsmpc-gui) â ç¨äº mpd ç gtk åç«¯.
- [Polaris](https://github.com/agersant/polaris) â é³ä¹æµåªä½åºç¨ç¨åº. 
- [Spotify TUI](https://github.com/Rigellute/spotify-tui) â ä¸ä¸ªç¨ Rust ç¼åçç¨äºç»ç«¯ç Spotify å®¢æ·ç«¯. 
- [Spotifyd](https://github.com/Spotifyd/spotifyd) â ä½ä¸º UNIX å®æ¤ç¨åºè¿è¡çå¼æº Spotify å®¢æ·ç«¯. 
  
### å å¯æ°å­è´§å¸

- [Bitcoin Satoshi's Vision](https://github.com/brentongunning/rust-sv) â ç¨äºå¤çæ¯ç¹å¸ SV ç Rust åº.
- [cardano-cli](https://github.com/input-output-hk/cardano-cli) â å¡å°è¾¾è¯ºå½ä»¤è¡çé¢ (CLI)
- [ChainX](https://github.com/chainx-org/ChainX) â Polkadot ä¸å®å¨å»ä¸­å¿åçé¾é´å å¯èµäº§ç®¡ç.
- [CITA](https://github.com/citahub/cita) â é¢åä¼ä¸ç¨æ·çé«æ§è½åºåé¾åæ ¸.
- [coinbase-pro-rs](https://github.com/inv2004/coinbase-pro-rs) â Rust ä¸­ç Coinbase pro å®¢æ·ç«¯ï¼æ¯æåæ­¥ / å¼æ­¥ / websocket 
- [ethaddrgen](https://github.com/Limeth/ethaddrgen) â ç¨ Rust å¶ä½çèªå®ä¹ä»¥å¤ªåèå°åçæå¨ 
- [Grin](https://github.com/mimblewimble/grin/) â MimbleWimble åè®®çæ¼å
- [hdwallet](https://github.com/jjyr/hdwallet) â BIP-32 HD é±åç¸å³çå¯é¥æ¨å¯¼å®ç¨ç¨åº.
- [Holochain](https://github.com/holochain/holochain) â åºåé¾çå¯æ©å± P2P æ¿ä»£æ¹æ¡ï¼éç¨äºæ¨ä¸ç´æ³è¦æå»ºçææåå¸å¼åºç¨ç¨åº. æ§ä»åºçé¾æ¥æ¯ [this](https://github.com/holochain/holochain-rust) ä¸åç»´æ¤.[ibc-rs](https://github.com/informalsystems/ibc-rs) - Rust çå®ç° [Interblockchain Communication](https://xn--ibc-3h3e109w.org/) åè®®
- [infincia/bip39-rs](https://github.com/infincia/bip39-rs) â BIP39 ç Rust å®ç°.
- [Joystream](https://github.com/Joystream/joystream) â ä¸ä¸ªç¨æ·ç®¡ççè§é¢å¹³å° 
- [Diem](https://github.com/diem/diem) â Diem çä½¿å½æ¯å»ºç«ä¸ä¸ªç®åçå¨çè´§å¸åéèåºç¡è®¾æ½ï¼ä¸ºæ°åäº¿äººèµè½.
- [Lighthouse](https://github.com/sigp/lighthouse) â Rust Ethereum 2.0 å®¢æ·ç«¯
- [near/nearcore](https://github.com/near/nearcore) â ç¨äºä½ç«¯ç§»å¨è®¾å¤çå»ä¸­å¿åæºè½åçº¦å¹³å°.
- [Nervos CKB](https://github.com/nervosnetwork/ckb) â Nervos CKB æ¯ä¸ä¸ªå¬å±çåè®¸å¯åºåé¾ï¼æ¯ Nervos ç½ç»çå¬å±ç¥è¯å±.
- [Nimiq](https://github.com/nimiq/core-rs) â Nimiq èç¹ç Rust å®ç°
- [Parity-Bitcoin](https://github.com/paritytech/parity-bitcoin) â Parity æ¯ç¹å¸å®¢æ·ç«¯
- [Parity-Bridge](https://github.com/paritytech/parity-bridge) â ä»»ä½ä¸¤ä¸ªåºäºä»¥å¤ªåçç½ç»ä¹é´çæ¡¥æ¢
- [Parity-Ethereum](https://github.com/openethereum/openethereum) â å¿«éãè½»ä¾¿ãå¼ºå¤§çä»¥å¤ªåå®¢æ·ç«¯
- [Parity-Zcash](https://github.com/paritytech/parity-zcash) â Zcash åè®®ç Rust å®ç°
- [Phala-Network/phala-blockchain](https://github.com/Phala-Network/phala-blockchain) â åºäº Intel SGX å Substrate çæºå¯æºè½åçº¦åºåé¾
- [Polkadot](https://github.com/paritytech/polkadot) â å·æéä¸­å®å¨æ§çå¼æå¤é¾ææ¯
- [rbtc](https://github.com/lucawen/rbtc) â å° BTC è½¬æ¢ä¸ºä»»ä½è´§å¸ï¼åä¹äº¦ç¶. 
- [rust-cardano](https://github.com/input-output-hk/rust-cardano) â Cardano åè¯­ãå©æåç¸å³åºç¨ç¨åºç Rust å®ç°
- [Substrate](https://github.com/paritytech/substrate) â ç¨ Rust ç¼åçéç¨æ¨¡åååºåé¾æ¨¡æ¿
- [tendermint-rs](https://github.com/informalsystems/tendermint-rs) - Tendermint åºåé¾æ°æ®ç»æåå®¢æ·ç«¯ç Rust å®ç°
- [wagyu](https://github.com/AleoHQ/wagyu) [[wagyu](https://crates.io/crates/wagyu)] â ç¨äºçæå å¯è´§å¸é±åç Rust åº
- [zcash](https://github.com/zcash/zcash) â Zcash æ¯ âZerocashâ åè®®çå®ç°.
- [YeeCo yeeroot](https://github.com/yeeco/yeeroot) â YeeCo yeeroot æ¯ä¸ä¸ªæ éè®¸å¯ãå®å¨ãé«æ§è½åå¯æ©å±çå¬å±åºåé¾å¹³å°ï¼ç±åºäº Rust ç¼åç PoW å±è¯çå¨åçææ¯æä¾æ¯æ
  
### æ°æ®åº

- [indradb](https://crates.io/crates/indradb) â åºäº Rust çå¾å½¢æ°æ®åº 
- [Materialize](https://github.com/MaterializeInc/materialize) - ç± Timely Dataflow æä¾æ¯æçæµå¼ SQL æ°æ®åºï¼heavy_dollar_sign
- [noria](https://crates.io/crates/noria) â ç¨äº Web åºç¨ç¨åºåç«¯çå¨æååãé¨åç¶æçæ°æ®æµ
- [Lucid](https://github.com/lucid-kv/lucid) â High performance and distributed KV store accessible through a HTTP API.
- [ParityDB](https://github.com/paritytech/parity-db) â å¿«éå¯é çæ°æ®åºï¼éå¯¹è¯»æä½è¿è¡äºä¼å
- [PumpkinDB](https://github.com/PumpkinDB/PumpkinDB) â äºä»¶æº¯æºæ°æ®åºå¼æ 
- [seppo0010/rsedis](https://github.com/seppo0010/rsedis) â Rust ä¸­ç Redis éæ°å®ç° 
- [Skytable](https://github.com/skytable/skytable) â å¤æ¨¡å NoSQL æ°æ®åº 
- [tikv](https://github.com/tikv/tikv) â Rust ä¸­çåå¸å¼ KV æ°æ®åº 
- [sled](https://crates.io/crates/sled) âï¼æµè¯çï¼ç°ä»£åµå¥å¼æ°æ®åº
- [TerminusDB](https://github.com/terminusdb/terminusdb-store) - å¼æºå¾å½¢æ°æ®åºåææ¡£å­å¨
  
### æ¨¡æå¨

- [kondrak/rust64](https://github.com/kondrak/rust64) 
- [Ruffle](https://github.com/ruffle-rs/ruffle) â Ruffle æ¯ç¨ Rust ç¼ç¨è¯­è¨ç¼åç Adobe Flash Player æ¨¡æå¨. Ruffle ä½¿ç¨ WebAssembly é¢åæ¡é¢å Web.
- [Gekkio/mooneye-gb](https://github.com/Gekkio/mooneye-gb) 
- [mvdnes/rboy](https://github.com/mvdnes/rboy)
- [NivenT/RGB](https://github.com/nivent/RGB) 
- [mohanson/gameboy](https://github.com/mohanson/gameboy) â å¨åè½è·¨å¹³å° GameBoy æ¨¡æå¨. æ°¸è¿çç·å­©ï¼
- [michelhe/rustboyadvance-ng](https://github.com/michelhe/rustboyadvance-ng) - RustboyAdvance-ng æ¯ä¸æ¬¾ Gameboy Advance æ¨¡æå¨ï¼å·ææ¡é¢ãå®åå [WebAssembly](https://michelhe.github.io/rustboyadvance-ng/) æ¯æ.
- [iamsix/oxidenes](https://github.com/iamsix/oxidenes)
- [koute/pinky](https://github.com/koute/pinky) 
- [pcwalton/sprocketnes](https://github.com/pcwalton/sprocketnes)
- [Amjad50/plastic](https://github.com/Amjad50/plastic) â plastis æ¯ä¸ä¸ªç¨ Rust æå»ºçå¨åè½ NES æ¨¡æå¨.
- [rustation-ng](https://gitlab.com/flio/rustation-ng/) â ä½¿ç¨ Rust ç Playstation æ¨¡æå¨
- [pacmancoder/rustzx](https://github.com/pacmancoder/rustzx) 
- [rodrigorc/raze](https://github.com/rodrigorc/raze) â å¯¹äº WebAssemblyï¼ [live version here](https://rodrigorc.github.io/raze/) * èæç·å­©
- [emu-rs/rustual-boy](https://github.com/emu-rs/rustual-boy) 
- [mohanson/i8080](https://github.com/mohanson/i8080) â Rust ç Intel 8080 cpu æ¨¡æå¨ 
  
### æ¸¸æ

- [lifthrasiir/angolmois-rust](https://github.com/lifthrasiir/angolmois-rust) â ä¸æ¬¾æ¯æ BMS æ ¼å¼çæç®é³ä¹è§é¢æ¸¸æ
- [citybound](https://github.com/citybound/citybound) - ä½ åºå¾çåå¸æ¨¡æ
- [schulke-214/connect-four](https://github.com/schulke-214/connect-four) â ä¸ä¸ªç®åçè¿æ¥åä¸ªå®ç°.
- [doukutsu-rs](https://github.com/doukutsu-rs/doukutsu-rs) â å¯¹ Cave Story å¼æç Rust éæ°å®ç°ï¼å¹¶è¿è¡äºä¸äºå¢å¼º.
- [rsaarelm/magog](https://github.com/rsaarelm/magog) â Rust ä¸­ç roguelike æ¸¸æ
- [schulke-214/rsnake](https://github.com/schulke-214/rsnake) â ç¨ Rust ç¼åç Snake.
- [soydos](https://github.com/soydos/pusoy_dos2) â Pusoy Dos ç wasm å®ç°
- [cristicbz/rust-doom](https://github.com/cristicbz/rust-doom) â Doom çæ¸²æå¨ï¼å¯è½ä¼åå±æä¸ºä¸æ¬¾å¯ç©çæ¸¸æ 
- [Thinkofname/rust-quake](https://github.com/Thinkofname/rust-quake) â Rust ä¸­çå°éå°å¾æ¸²æå¨
- [rhex](https://github.com/dpc/rhex) â å­è¾¹å½¢ ascii roguelike
- [garkimasera/rusted-ruins](https://github.com/garkimasera/rusted-ruins) - å·æåç´ èºæ¯çå¯æ©å±å¼æ¾ä¸çæµæ°æ¸¸æ
- [Veloren](https://gitlab.com/veloren/veloren) â ä¸ä¸ªå¼æ¾ä¸çãå¼æºçå¤äººä½ç´  RPG æ¸¸æï¼ç®åå¤äº alpha å¼åé¶æ®µ
- [swatteau/sokoban-rs](https://github.com/swatteau/sokoban-rs) â æ¨ç®±å­å®ç°
- [aleshaleksey/TGWM](https://github.com/aleshaleksey/TGWM) â å·æååå¶æºå¶ç RPGï¼æ­£å¨è¿è¡ä¸­ï¼
- [ozkriff/zemeroth](https://github.com/ozkriff/zemeroth) â ä¸æ¬¾å°å 2D ååå¶å­è§ç­ç¥æ¸¸æ
- [Zone of Control](https://github.com/ozkriff/zoc) â ååå¶å­è§ç­ç¥æ¸¸æ 
- [phantomion/snake_game](https://github.com/phantomion/snake_game) - ç¨ Rust ç¼åçç®åç»ç«¯èæ¸¸æ.

### å¾å½¢å¤ç

- [Limeth/euclider](https://github.com/Limeth/euclider) â å®æ¶ 4D CPU åçº¿è¿½è¸ªå¨
- [RazrFalcon/resvg](https://github.com/RazrFalcon/resvg) â ä¸ä¸ª SVG æ¸²æåº.
- [ivanceras/svgbob](https://github.com/ivanceras/svgbob) â å° ASCII å¾è½¬æ¢ä¸º SVG å¾å½¢ 
- [RazrFalcon/svgcleaner](https://github.com/RazrFalcon/svgcleaner) â æ´ç SVG å¾å½¢
- [Twinklebear/tray_rust](https://github.com/Twinklebear/tray_rust) â åçº¿è¿½è¸ªå¨
- [turnage/valora](https://crates.io/crates/valora) â çæç¾æ¯å¾ä¹¦é¦ 
- [mikigraf/Image-Processing-CLI-in-Rust](https://github.com/mikigraf/Image-Processing-CLI-in-Rust) â ç¨äºå¤çå¾åãçæç´æ¹å¾ç CLI. 

### å·¥ä¸èªå¨å

- [locka99/opcua](https://github.com/locka99/opcua) â  [OPC UA](https://opcfoundation.org/about/opc-technologies/opc-ua/) å¾ä¹¦é¦.
- [slowtec/tokio-modbus](https://github.com/slowtec/tokio-modbus) - ä¸ç§ [tokio](https://tokio.rs/)-based [modbus](https://modbus.org/) å¾ä¹¦é¦. 
- [BiancoRoyal/modbus-iiot-rust](https://github.com/BiancoRoyal/modbus-iiot-rust) â çº¯é [modbus](https://modbus.org/) æ²¡æææ´å°ä¾èµçåº.
  
### å¯è§å¯æ§å·¥å·

- [timberio/vector](https://github.com/timberio/vector) â é«æ§è½ãæ¥å¿ãææ åäºä»¶è·¯ç±å¨.
- [Mnwa/gtsa](https://github.com/Mnwa/gtsa) â å° gelf æ¶æ¯ï¼Graylog çæ¶æ¯ï¼ä»£çå° Sentry çç®åè§£å³æ¹æ¡
- [OpenTelemetry](https://crates.io/crates/opentelemetry) â OpenTelemetry æä¾ä¸ç» APIãåºãä»£çåæ¶éå¨æå¡ï¼ä»¥ä»æ¨çåºç¨ç¨åºä¸­æè·åå¸å¼è·è¸ªåææ . æ¨å¯ä»¥ä½¿ç¨ PrometheusãJaeger åå¶ä»å¯è§å¯æ§å·¥å·åæå®ä»¬.

### æä½ç³»ç»

- [nebulet/nebulet](https://github.com/nebulet/nebulet) â å®ç°å¨ Ring 0 ä¸­è¿è¡ç WebAssemblyâç¨æ·æ¨¡å¼â çå¾®åæ ¸.
- [redox-os/redox](https://gitlab.redox-os.org/redox-os/redox) 
- [thepowersgang/rust_os](https://github.com/thepowersgang/rust_os)
- [tock/tock](https://github.com/tock/tock) â éç¨äºåºäº Cortex-M çå¾®æ§å¶å¨çå®å¨åµå¥å¼æä½ç³»ç»

### çäº§è½å

- [espanso](https://github.com/federico-terzi/espanso) â ä¸ä¸ªç¨ Rust ç¼åçè·¨å¹³å°ææ¬æ©å±å¨ [eureka](https://crates.io/crates/eureka) â æ éç¦»å¼ç»ç«¯å³å¯è¾å¥åå­å¨æ¨çæ³æ³ç CLI å·¥å·
- [pier-cli/pier](https://github.com/pier-cli/pier) â ç¨äºç®¡çï¼æ·»å ãæç´¢åæ°æ®ç­ï¼ææåè¡ç¨åºãèæ¬ãå·¥å·å CLI çä¸­å¤®å­å¨åº
- [subilo](https://github.com/Bansco/subilo) - æç»­é¨ç½²ä»£ç

### å®å¨å·¥å·

- [kpcyrd/authoscope](https://github.com/kpcyrd/authoscope) â ä¸ä¸ªå¯ç¼åèæ¬çç½ç»è®¤è¯ç ´è§£å¨
- [lethe](https://github.com/kostassoid/lethe) â å®å¨çè·¨å¹³å°é©±å¨å¨æ¦é¤å®ç¨ç¨åº 
- [arvancloud/libinjection-rs](https://github.com/arvancloud/libinjection-rs) â Rust ç»å® [libinjection](https://github.com/client9/libinjection)
- [ripasso](https://github.com/cortex/ripasso/) â å¯ç ç®¡çå¨ï¼ä¸ pass å¼å®¹çæä»¶ç³»ç»
- [kpcyrd/rshijack](https://github.com/kpcyrd/rshijack) â ä¸ä¸ª TCP è¿æ¥å«æèï¼å¯¹ shijack è¿è¡ Rust éå 
- [rustscan/rustscan](https://github.com/RustScan/RustScan) â ä½¿ç¨æ­¤ç«¯å£æ«æå·¥å·ä½¿ Nmap æ´å¿«
- [kpcyrd/sniffglue](https://github.com/kpcyrd/sniffglue) â ä¸ä¸ªå®å¨çå¤çº¿ç¨æ°æ®ååæ¢å¨
- [kpcyrd/sn0int](https://github.com/kpcyrd/sn0int) â åèªå¨ OSINT æ¡æ¶ååç®¡çå¨   

### ç³»ç»å·¥å·

- [ajeetdsouza/zoxide](https://github.com/ajeetdsouza/zoxide/) â ä¸ç§å¿«éæ¿ä»£ `cd` çæ¹æ³ï¼å¯ä»¥å­¦ä¹ ä½ çä¹ æ¯
- [bandwhich](https://github.com/imsnif/bandwhich) â ç»ç«¯å¸¦å®½å©ç¨å·¥å·
- [brocode/fblog](https://github.com/brocode/fblog) â å°åå½ä»¤è¡ JSON æ¥å¿æ¥çå¨ 
- [buster/rrun](https://github.com/buster/rrun) â Linux çå½ä»¤å¯å¨å¨ï¼ç±»ä¼¼äº gmrun
- [cristianoliveira/funzzy](https://github.com/cristianoliveira/funzzy) â åå¯åçå¯éç½®æä»¶ç³»ç»è§å¯å¨ [entr](http://eradman.com/entrproject/) 
- [dalance/procs](https://github.com/dalance/procs) â Rust ç¼åç âpsâ çç°ä»£æ¿ä»£å
- [diskonaut](https://github.com/imsnif/diskonaut) â ç»ç«¯å¯è§åç£çç©ºé´å¯¼èªå¨
- [dust](https://github.com/bootandy/dust) â æ´ç´è§ç du çæ¬
- [ddh](https://github.com/darakian/ddh) â å¿«ééå¤æä»¶æ¥æ¾å¨
- [fselect](https://crates.io/crates/fselect) â ä½¿ç¨ç±»ä¼¼ SQL çæ¥è¯¢æ¥æ¾æä»¶ 
- [gitui](https://github.com/extrawurst/gitui) - ç¨ Rust ç¼åç git å¿«éç»ç«¯å®¢æ·ç«¯.
- [k0pernicus/zou](https://github.com/k0pernicus/zou) â ä¸è½½å éå¨
- [Kondo](https://github.com/tbillington/kondo) - ç¨äºå é¤è½¯ä»¶é¡¹ç®å·¥ä»¶ååæ¶ç£çç©ºé´ç CLI å GUI å·¥å·
- [lotabout/rargs](https://github.com/lotabout/rargs) [[rargs](https://crates.io/crates/rargs)] â æ¯ææ¨¡å¼å¹éç xargs + awk
- [lotabout/skim](https://github.com/lotabout/skim) â çº¯éçæ¨¡ç³åæ¯å¨
- [mitnk/cicada](https://github.com/mitnk/cicada) â ä¸ä¸ªç±»ä¼¼ bash ç Unix shell
- [mmstick/concurr](https://github.com/mmstick/concurr) â å¸¦æå®¢æ·ç«¯ - æå¡å¨æ¶æç GNU Parallel çæ¿ä»£æ¹æ¡
- [mmstick/fontfinder](https://github.com/mmstick/fontfinder) â ç¨äºé¢è§åå®è£ Google å­ä½ç GTK3 åºç¨ç¨åº
- [mmstick/parallel](https://github.com/mmstick/parallel) â éæ°å®ç° GNU Parallel
- [mmstick/tv-renamer](https://github.com/mmstick/tv-renamer) â å¸¦æå¯é GTK3 åç«¯ççµè§å§éå½ååºç¨ç¨åº. 
- [nushell/nushell](https://github.com/nushell/nushell) â ä¸ä¸ªæ°åShell. 
- [organize-rt](https://gitlab.com/FixFromDarkness/organize-rt) â æ ¹æ®æ­£åè¡¨è¾¾å¼è§åç»ç»æä»¶ï¼é»è®¤ä¸ºæä»¶æ©å±åï¼.
- [orhun/kmon](https://github.com/orhun/kmon) â Linux åæ ¸ç®¡çå¨åæ´»å¨çè§å¨ 
- [Peltoche/lsd](https://github.com/Peltoche/lsd) â ä¸ä¸ª ls æå¾å¤æ¼äº®çé¢è²åå¾æ£çå¾æ  
- [ogham/exa](https://github.com/ogham/exa) â 'ls' çæ¿ä»£å 
- [pop-os/debrep](https://github.com/pop-os/debrepbuild) â ç¨äºæå»ºåç®¡ç APT å­å¨åºç APT å­å¨åºå·¥å·
- [pop-os/popsicle](https://github.com/pop-os/popsicle) â GTK3 å CLI å®ç¨ç¨åºï¼ç¨äºå¹¶è¡å·æ°å¤ä¸ª USB è®¾å¤
- [pueue](https://github.com/nukesor/pueue) â ç®¡çæ¨é¿æ¶é´è¿è¡ç shell å½ä»¤.
- [Luminarys/synapse](https://github.com/Luminarys/synapse) â çµæ´»ä¸å¿«éç BitTorrent å®æ¤è¿ç¨. 
- [pop-os/system76-power](https://github.com/pop-os/system76-power/) â å¸¦æ CLI å·¥å·ç Linux çµæºç®¡çå®æ¤è¿ç¨ï¼DBus æ¥å£ï¼.
- [mxseev/logram](https://github.com/mxseev/logram) â å°æ¥å¿æä»¶çæ´æ°æ¨éå° Telegram
- [redox-os/ion](https://github.com/redox-os/ion) â ä¸ä¸ä»£ç³»ç»å¤å£³ 
- [jamesbirtles/hotkey-rs](https://github.com/jamesbirtles/hotkey-rs) â å¨ Rust ä¸­æ¶å¬å¨å±ç­é®çåº
- [nivekuil/rip](https://github.com/nivekuil/rip) - ä¸ç§å®å¨ä¸ç¬¦åäººä½å·¥ç¨å­¦çæ¿ä»£`rm` 
- [sharkdp/bat](https://github.com/sharkdp/bat) â æç¿èç cat(1) åéä½. 
- [sharkdp/fd](https://github.com/sharkdp/fd) â ä¸ç§ç®åãå¿«éä¸ç¨æ·åå¥½çæ¥æ¾æ¿ä»£æ¹æ¡.
- [sitkevij/hex](https://github.com/sitkevij/hex) â å½©è²ç hexdump ç»ç«¯å®ç¨ç¨åº.
- [slai11/goto](https://github.com/slai11/goto) â è·³è½¬å°ç´¢å¼ç®å½çç®åä¸ç¨æ·åå¥½çæ¹å¼.
- [m4b/bingrep](https://github.com/m4b/bingrep) â éè¿æ¥èªåç§æä½ç³»ç»åä½ç³»ç»æçäºè¿å¶æä»¶è¿è¡ Grepsï¼å¹¶ä¸ºå®ä»¬çè². 
- [uutils/coreutils](https://github.com/uutils/coreutils) â GNU coreutils çè·¨å¹³å° Rust éå
- [watchexec](https://github.com/watchexec/watchexec) â æ§è¡å½ä»¤ä»¥ååºæä»¶ä¿®æ¹ 
- [XAMPPRocky/tokei](https://github.com/XAMPPRocky/tokei) â è®¡ç®ä»£ç è¡æ° 
- [yake](https://crates.io/crates/yake) â Yake æ¯ä¸ä¸ªåºäº yaml æä»¶çä»»å¡è¿è¡å¨
- [ytop](https://github.com/cjbassi/ytop) - ä¸ä¸ªç¨ Rust ç¼åç TUI ç³»ç»çè§å¨ 
- [cocom](https://github.com/LamdaLamdaLamda/cocom) - çº¯ç²¹ç¨ Rust ç¼åç NTP å®¢æ·ç«¯. 

### æå­ç¼è¾å¨

- [amp](https://amp.rs/) â å Vi/Vim çå¯å. 
- [gchp/iota](https://github.com/gchp/iota) â ä¸ä¸ªç®åçææ¬ç¼è¾å¨
- [ilai-deutel/kibi](https://github.com/ilai-deutel/kibi) â å·æè¯­æ³é«äº®ãå¢éæç´¢ç­åè½çå°å (â¤1024 LOC) ææ¬ç¼è¾å¨.
- [vamolessa/pepper](https://github.com/vamolessa/pepper) [[pepper](https://crates.io/crates/pepper)] â ä¸ä¸ªèªä»¥ä¸ºæ¯çæ¨¡å¼ç¼è¾å¨ï¼å¯ç®åä»ç»ç«¯è¿è¡çä»£ç ç¼è¾
- [mathall/rim](https://github.com/mathall/rim) â ç¨ Rust ç¼åçç±»ä¼¼ Vim çææ¬ç¼è¾å¨
- [ox](https://github.com/curlpipe/ox) â å¨ç»ç«¯ä¸­è¿è¡çç¬ç« Rust ææ¬ç¼è¾å¨ï¼
- [Remacs](https://github.com/remacs/remacs) â ç¤¾åºé©±å¨ç Emacs å° Rust çç§»æ¤.
- [xi-editor](https://github.com/xi-editor/xi-editor) â ä¸ä¸ªç°ä»£ç¼è¾å¨ï¼åç«¯æ¯ç¨ Rust ç¼åç.
- [xray](https://github.com/atom-archive/xray) â å®éªæ§çä¸ä¸ä»£åºäºçµå­çææ¬ç¼è¾å¨. 

### ææ¬å¤ç

- [cpc](https://github.com/probablykasper/cpc) - è§£æåè®¡ç®æ°å­¦å­ç¬¦ä¸²ï¼æ¯æåä½ååä½è½¬æ¢ï¼ä» â1+2â å°â1% çååï¼1 åå¹´ / 14!s å°å¬é / å°æ¶ï¼â.
- [grex](https://github.com/pemistahl/grex) â ç¨äºä»ç¨æ·æä¾çæµè¯ç¨ä¾çææ­£åè¡¨è¾¾å¼çå½ä»¤è¡å·¥å·ååº
- [dmerejkowsky/ruplacer](https://github.com/dmerejkowsky/ruplacer) â å¨æºæä»¶ä¸­æ¥æ¾åæ¿æ¢ææ¬
- [ripgrep](https://crates.io/crates/ripgrep) â ç»åäº Silver Searcher çå¯ç¨æ§å grep çåå§éåº¦
- [phiresky/ripgrep-all](https://github.com/phiresky/ripgrep-all) â ripgrepï¼è¿å¯ä»¥æç´¢ PDFãçµå­ä¹¦ãOffice ææ¡£ãzipãtar.gz ç­.
- [replicadse/complate](https://github.com/replicadse/complate) â ä¸ç§ç»ç«¯åææ¬æ¨¡æ¿å·¥å·ï¼ç¨äºæ ååæ¶æ¯ï¼å¦ GIT æäº¤ï¼. 
- [sd](https://crates.io/crates/sd) â ç´è§çæ¥æ¾åæ¿æ¢ CLI
- [lavifb/todo_r](https://github.com/lavifb/todo_r) â ç¨ä¸ä¸ªå½ä»¤æ¥æ¾ææ TODO ç¬è®°ï¼ 
- [whitfin/runiq](https://github.com/whitfin/runiq) â ä»æªæåºçè¾å¥ä¸­è¿æ»¤éå¤è¡çæææ¹æ³.
- [whitfin/bytelines](https://github.com/whitfin/bytelines) â å°è¾å¥è¡è¯»åä¸ºå­èçä»¥æé«æç.
- [vishaltelangre/ff](https://github.com/vishaltelangre/ff) â æåç§°æ¥æ¾æä»¶ (ff)ï¼ 
- [xsv](https://crates.io/crates/xsv) â ä¸ä¸ªå¿«éç CSV å½ä»¤è¡å·¥å·ï¼åçãç´¢å¼ãéæ©ãæç´¢ãéæ ·ç­ï¼
- [Lisprez/so_stupid_search](https://github.com/Lisprez/so_stupid_search) â ä¸ä¸ªç®åå¿«éçäººç±»å­ç¬¦ä¸²æç´¢å·¥å·

### å¾åå¤ç

- [Imager](https://github.com/imager-io/imager) â èªå¨å¾åä¼å.

### å®ç¨å·¥å·

- [aleshaleksey/AZDice](https://github.com/aleshaleksey/AZDice) â æ¡é¢å®¶åº­é¿éåçéª°å­æåååçæå¨. 
- [yaa110/cb](https://github.com/yaa110/cb) â ç®¡çåªè´´æ¿çå½ä»¤è¡çé¢ 
- [brycx/checkpwn](https://github.com/brycx/checkpwn) â ä¸ä¸ª Have I Being Pwned (HIBP) å½ä»¤è¡å®ç¨å·¥å·ï¼å¯è®©æ¨è½»æ¾æ£æ¥è¢«çç¨çå¸æ·åå¯ç .
- [vamolessa/copycat](https://github.com/vamolessa/copycat) [[copycat](https://crates.io/crates/copycat)] â ä¸ä¸ªç®åçåªè´´æ¿ cli çé¢ï¼éç¨äºå·æææ¬å bmp æ¯æççªå£
- [evansmurithi/cloak](https://github.com/evansmurithi/cloak) â å½ä»¤è¡ OTPï¼ä¸æ¬¡æ§å¯ç ï¼èº«ä»½éªè¯å¨åºç¨ç¨åº. 
- [replydev/cotp](https://github.com/replydev/cotp) - ä¸å¤é¨å¤ä»½å¼å®¹çå¼å¾ä¿¡èµçå å¯ä¸æ¬¡æ§å¯ç éªè¯å¨åºç¨ç¨åº. 
- [rustdesk/rustdesk](https://github.com/rustdesk/rustdesk) - è¿ç¨æ¡é¢åºç¨ç¨åº. 
- [arthrp/consoletimer](https://github.com/arthrp/consoleTimer) â ç»ç«¯çç®åè®¡æ¶å¨.
- [tversteeg/emplace](https://github.com/tversteeg/emplace) â å¨å¤å°æºå¨ä¸åæ­¥å·²å®è£çå
- [unrelentingtech/freepass](https://github.com/unrelentingtech/freepass) â é«çº§ç¨æ·çåè´¹å¯ç ç®¡çå¨.
- [yoannfleurydev/gitweb](https://github.com/yoannfleurydev/gitweb) â å¨æµè§å¨ä¸­æå¼å½åè¿ç¨å­å¨åº.
- [mme](https://github.com/GoberInfinity/mme) â å½ä»¤è¡å·¥å·æ¥è®°ä½æ¨ææ¶å¿è®°çå½ä»¤. 
- [raftario/licensor](https://github.com/raftario/licensor) â å°è®¸å¯è¯åå¥æ åè¾åº
- [arthrp/quick-skeleton](https://github.com/arthrp/quick-skeleton) â é¡¹ç®èææ¶å·¥å·ï¼ç±»ä¼¼äº Yeoman å Slush. 
- [repoch](https://github.com/lucawen/repoch) â å°çºªåè½¬æ¢ä¸ºæ¥ææ¶é´ï¼å°æ¥ææ¶é´è½¬æ¢ä¸ºçºªå 
- [whitfin/s3-concat](https://github.com/whitfin/s3-concat) â ä½¿ç¨çµæ´»æ¨¡å¼è¿ç¨è¿æ¥ Amazon S3 æä»¶çå½ä»¤è¡å·¥å·.
- [whitfin/s3-meta](https://github.com/whitfin/s3-meta) â ç¨äºæ¶éæå³ Amazon S3 å­å¨æ¡¶çåæ°æ®çå½ä»¤è¡å·¥å·.
- [whitfin/s3-utils](https://github.com/whitfin/s3-utils) â ä¸ä¸ªåå«åºäº Amazon S3 çå®ç¨ç¨åºçå°å·¥å·ï¼å¯æä¾é¢å¤çä¾¿å© API.
- [gorros/s3-edit-rs](https://github.com/gorros/s3-edit-rs) â ç´æ¥å¨ Amazon S3 ä¸ç¼è¾æä»¶çå½ä»¤è¡å·¥å·.
- [fcsonline/tmux-thumbs](https://github.com/fcsonline/tmux-thumbs) â ç¨ Rust ç¼åç tmux-finger çéªçµè¬å¿«éçæ¬ï¼å vimium/vimperator ä¸æ ·å¤å¶ / ç²è´´ tmux.
- [amar-laksh/workstation](https://github.com/amar-laksh/workstation) â ä¸ä¸ªå½ä»¤è¡å·¥å·ï¼å¯å¸®å©æ¨ç®¡çå·¥ä½ç«ï¼è®©æ¨è¿ç¦»å±å¹ãå¨æ¨ä¸å¨æ¶éå®å±å¹ä»¥åä½¿ç¨ OPENCV è¿è¡å¶ä»æä½ï¼
- [guoxbin/dtool](https://github.com/guoxbin/dtool) â ä¸ä¸ªæç¨çå½ä»¤è¡å·¥å·éåï¼ç¨äºåå©å¼åï¼åæ¬è½¬æ¢ãç¼è§£ç å¨ãæ£åãå å¯ç­.
- [nomino](https://github.com/yaa110/nomino) â å¼åäººåæ¹ééå½åå®ç¨ç¨åº 
- [barberousse](https://github.com/zeapo/barberousse) â AWS Secrets Manager ç¼è¾å¨ 
- [vamolessa/verco](https://github.com/vamolessa/verco) [[verco](https://crates.io/crates/verco)] â ä¸ä¸ªç®åç Git/Hg tui å®¢æ·ç«¯ï¼ä¸æ³¨äºé®çå¿«æ·é®
  
### è§é¢

- [Phate6660/rsmpv](https://github.com/Phate6660/rsmpv) â MPV æ§å¶å¨ï¼éè¦å¨ MPV ä¸­å¯ç¨ IPC.
- [tgotwig/vidmerger](https://github.com/tgotwig/vidmerger) â ffmpeg çåè£å¨ï¼å¯ç®åå¤ä¸ªè§é¢çåå¹¶
- [xiph/rav1e](https://github.com/xiph/rav1e) â æå¿«ãæå®å¨ç AV1 ç¼ç å¨.
- [yuvadm/slingr](https://github.com/yuvadm/slingr) â ä¸ä¸ªç®åç CLIï¼ç¨äºéè¿æ¬å°ç½ç»å°åªä½æä»¶æµå¼ä¼ è¾å° UPnP åªä½æ¸²æå¨
- [yuvadm/streamlib](https://github.com/streamlib/streamlib) â ä»å½ä»¤è¡æ­æ¾æ¨æåæ¬¢çå®æ¶è§é¢åé³é¢æµ

### èæåææ¯

- [firecracker-microvm/firecracker](https://github.com/firecracker-microvm/firecracker) â ç¨äºå®¹å¨å·¥ä½è´è½½çè½»éçº§èææº [Firecracker Microvm](https://firecracker-microvm.github.io/)
- [oracle/railcar](https://github.com/oracle/railcar) â Rust ä¸­ç±»ä¼¼ Docker çå®¹å¨ OCI è¿è¡æ¶å®ç°
- [tailhook/vagga](https://github.com/tailhook/vagga) â ä¸ä¸ªæ²¡æå®æ¤è¿ç¨çå®¹å¨åå·¥å·

### Web

- [Plume-org/Plume](https://github.com/Plume-org/Plume) â ActivityPub èååå®¢åºç¨ç¨åº
- [LemmyNet/lemmy](https://github.com/LemmyNet/lemmy) â èé¦å®å®çé¾æ¥èåå¨ / reddit åé

### Web Servers

- [mufeedvh/binserve](https://github.com/mufeedvh/binserve) â æå¿«çéæ Web æå¡å¨ï¼å¨åä¸ªäºè¿å¶æä»¶ä¸­å·æè·¯ç±ãæ¨¡æ¿åå®å¨æ§ï¼æ¨å¯ä»¥ä½¿ç¨é¶ä»£ç è¿è¡è®¾ç½® 
- [thecoshman/http](https://github.com/thecoshman/http) â è¯·æç®¡è¿äºä¸è¥¿ â ä¸ä¸ªåºæ¬ç http æå¡å¨ï¼ç¨äºå¿«éç®åå°æç®¡æä»¶å¤¹ 
- [svenstaro/miniserve](https://github.com/svenstaro/miniserve) â ä¸ä¸ªå°åçãèªåå«çè·¨å¹³å° CLI å·¥å·ï¼åè®¸æ¨åªè·åäºè¿å¶æä»¶å¹¶éè¿ HTTP æä¾ä¸äºæä»¶
- [TheWaWaR/simple-http-server](https://github.com/TheWaWaR/simple-http-server) â ç®åçéæ http æå¡å¨
- [wyhaya/see](https://github.com/wyhaya/see) â éæ HTTP æä»¶æå¡å¨
- [ronanyeah/rust-hasura](https://github.com/ronanyeah/rust-hasura) â Rust GraphQL æå¡å¨å¦ä½ç¨ä½è¿ç¨æ¨¡å¼çæ¼ç¤º [Hasura](https://hasura.io/) 
  
## å¼åå·¥å·
  
- [clippy](https://crates.io/crates/clippy)
- [clog-tool/clog-cli](https://github.com/clog-tool/clog-cli) â ä» git åæ°æ®çæåæ´æ¥å¿ ([conventional changelog](https://blog.thoughtram.io/announcements/tools/2014/09/18/announcing-clog-a-conventional-changelog-generator-for-the-rest-of-us.html)) 
- [dan-t/rusty-tags](https://github.com/dan-t/rusty-tags) â ä¸ºè´§ç©é¡¹ç®åå¶ææä¾èµé¡¹åå»º ctags/etags 
- [datanymizer/datanymizer](https://github.com/datanymizer/datanymizer) - å¼ºå¤§çæ°æ®åºå¿åå¨ï¼å·æçµæ´»çè§å
- [delta](https://crates.io/crates/git-delta) â git å diff è¾åºçè¯­æ³é«äº®å¨
- [dotenv-linter](https://github.com/dotenv-linter/dotenv-linter) â ç¨äº `.env` æä»¶ç Linter[frewsxcv/crate-deps](https://github.com/frewsxcv/crate-deps) â ä¸º crates.io ä¸æç®¡ç crate çæä¾èµå¾çå¾å
- [geiger](https://github.com/rust-secure-code/cargo-geiger) â ä¸ä¸ªç¨åºï¼ååºä¸å¨ Rust crate åå¶ææä¾èµé¡¹ä¸­ä½¿ç¨ä¸å®å¨ Rust ä»£ç ç¸å³çç»è®¡ä¿¡æ¯m/cargo-geiger/cargo-geiger/_build/latest?definitionId=1&branchName=master)
- [git-journal](https://github.com/saschagrunert/git-journal/) â Git æäº¤æ¶æ¯ååæ´æ¥å¿çææ¡æ¶ 
- [gstats](https://github.com/boonshift/gstats/) â ç¨äºæå°å½åç®å½ä¸ææ git å­å¨åºçå¼åäººåæ¹ä¾¿æè¦çå½ä»¤è¡å·¥å·
- [rust-lang/rustfix](https://github.com/rust-lang/rustfix) â èªå¨åºç¨ rustc æåºçå»ºè®®
- [just](https://github.com/casey/just) â ç¨äºç¹å®é¡¹ç®ä»»å¡çä¾¿æ·å½ä»¤è¿è¡å¨
- [mask](https://github.com/jakedeichert/mask) â ç±ä¸ä¸ªç®åç Markdown æä»¶å®ä¹ç CLI ä»»å¡è¿è¡å¨
- [Module Linker](https://github.com/fiatjaf/module-linker) âå¨ GitHub ç `mod`ã`use` å `extern crate` è¯­å¥ä¸­æ·»å  `<a>` é¾æ¥å°å¼ç¨çæ©å±.
- [ptags](https://github.com/dalance/ptags) â git å­å¨åºçå¹¶è¡éç¨ ctags åè£å¨ 
- [Racer](https://github.com/racer-rust/racer) â Rust çä»£ç å®æ 
- [rustfmt](https://github.com/rust-lang/rustfmt) â Rust ä»£ç æ ¼å¼åç¨åº
- [Rustup](https://github.com/rust-lang/rustup) â Rust å·¥å·é¾å®è£ç¨åº 
- [Rust Language Server](https://github.com/rust-lang/rls) â å¨åå°è¿è¡çæå¡å¨ï¼ä¸º IDEãç¼è¾å¨åå¶ä»å·¥å·æä¾æå³ Rust ç¨åºçä¿¡æ¯
- [Rust Regex Playground](https://2fd.github.io/rust-regex-playground/#method=find&regex=\w%2B&text=abc) â è¯ä¼° Rust æ­£åè¡¨è¾¾å¼ç Web å·¥å·
- [Rust Search Extension](https://github.com/huhu/rust-search-extension) â ä¸ä¸ªæ¹ä¾¿çæµè§å¨æ©å±ï¼ç¨äºå¨å°åæ ï¼å¤åè½æ¡ï¼ä¸­æç´¢ crate åææ¡£. 
- [artifact](https://github.com/vitiral/artifact) â ä¸ºå¼åäººåå¶ä½çè®¾è®¡ææ¡£å·¥å· 
- [semantic-rs](https://github.com/semantic-rs/semantic-rs) â èªå¨ crate åå¸
- [fw](https://github.com/brocode/fw) â å·¥ä½ç©ºé´çäº§åå©æ¨å¨ 
- [tinyrick](https://github.com/mcandre/tinyrick) ä¸ä¸ªåºæ¬çä»»å¡ä¾èµå·¥å·ï¼å¼ºè° Rust åè½èä¸æ¯åå§ shell å½ä»¤.
- [scriptisto](https://github.com/igor-petruk/scriptisto) ä¸ç§ä¸è¯­è¨æ å³ç âshebang è§£éå¨âï¼å®ä½¿æ¨è½å¤ç¨ç¼è¯è¯­è¨ç¼åä¸ä¸ªæä»¶èæ¬.
 
### ç³»ç»ç¼è¯

- [Cargo](https://crates.io/) â Rust åç®¡çå¨
- [cargo-benchcmp](https://crates.io/crates/cargo-benchcmp) â æ¯è¾ Rust å¾®åºåçå®ç¨ç¨åº 
- [cargo-bitbake](https://crates.io/crates/cargo-bitbake) â ä¸ä¸ªè´§ç©æ©å±ï¼å¯ä»¥å©ç¨ meta-rust ä¸­çç±»çæ BitBake éæ¹
- [cargo-cache](https://crates.io/crates/cargo-cache) - æ£æ¥ / ç®¡ç / æ¸çä½ çè´§ç©ç¼å­ï¼`~/.cargo/`/`${CARGO_HOME}`ï¼ï¼æå°å°ºå¯¸ç­
- [cargo-check](https://crates.io/crates/cargo-check) â `cargo rustc -- -Zno-trans` çåè£å¨ï¼å¦ææ¨åªéè¦æ­£ç¡®æ§æ£æ¥ï¼å®å¯ä»¥å¸®å©è¿è¡æ´å¿«çç¼è¯
- [cargo-count](https://crates.io/crates/cargo-count) â ååºæå³è´§ç©é¡¹ç®çæºä»£ç è®¡æ°åè¯¦ç»ä¿¡æ¯ï¼åæ¬ä¸å®å¨ç»è®¡æ°æ®
- [cargo-deb](https://crates.io/crates/cargo-deb) â çæäºè¿å¶ Debian è½¯ä»¶å
- [cargo-deps](https://crates.io/crates/cargo-deps) â æå»º Rust é¡¹ç®çä¾èµå¾
- [cargo-do](https://crates.io/crates/cargo-do) â è¿ç»­è¿è¡å¤ä¸ªè´§ç©å½ä»¤ 
- [cargo-ebuild](https://crates.io/crates/cargo-ebuild) â å¯ä»¥ä½¿ç¨æ å eclasses çæ ebuild çè´§ç©æ©å±
- [cargo-edit](https://crates.io/crates/cargo-edit) â åè®¸æ¨éè¿ä»å½ä»¤è¡è¯»å / åå¥ Cargo.toml æä»¶æ¥æ·»å åååºä¾èµé¡¹
- [cargo-generate](https://github.com/cargo-generate/cargo-generate) éè¿å©ç¨é¢åå­å¨ç git å­å¨åºä½ä¸ºæ¨¡æ¿æ¥çæ Rust é¡¹ç®.
- [cargo-get](https://crates.io/crates/cargo-get) - Cargo æä»¶å¯ä»¥è½»æ¾å°ä» Cargo.toml æä»¶ä¸­æ¥è¯¢ä¿¡æ¯ 
- [cargo-graph](https://crates.io/crates/cargo-graph) â æ´æ°äºå·æéå åè½ç `cargo-dot` åæ¯. æªç»´æ¤ï¼è¯·åé`cargo-deps` 
- [cargo-info](https://crates.io/crates/cargo-info) â ä»å½ä»¤è¡æ¥è¯¢ crates.io ä»¥è·å crates è¯¦ç»ä¿¡æ¯ 
- [cargo-license](https://crates.io/crates/cargo-license) â ä¸ä¸ªè´§ç©å­å½ä»¤ï¼ç¨äºå¿«éæ¥çææä¾èµé¡¹çè®¸å¯è¯.
- [cargo-make](https://crates.io/crates/cargo-make) â Rust ä»»å¡è¿è¡å¨åæå»ºå·¥å·. 
- [cargo-modules](https://crates.io/crates/cargo-modules) â ä¸ä¸ªè´§ç©æä»¶ï¼ç¨äºæ¾ç¤ºæ¿æ¡ç®±æ¨¡åçæ ç¶æ¦è§. 
- [cargo-multi](https://crates.io/crates/cargo-multi) â å¨å¤ä¸ªæ¿æ¡ç®±ä¸è¿è¡æå®çè´§ç©å½ä»¤
- [cargo-outdated](https://crates.io/crates/cargo-outdated) â å¨æ°çæ¬ç Rust ä¾èµé¡¹å¯ç¨æè¿æ¶æ¶æ¾ç¤º
- [cargo-release](https://crates.io/crates/cargo-release) â ç¨äºåå¸ git ç®¡ççè´§ç©é¡¹ç®ãæå»ºãæ è®°ãåå¸ãææ¡£åæ¨éçå·¥å· 
- [cargo-script](https://crates.io/crates/cargo-script) â è®©äººä»¬å¿«éãè½»æ¾å°è¿è¡ Rust âèæ¬âï¼å®å¯ä»¥å©ç¨ Cargo çåçæç³»ç»
- [cargo-testify](https://crates.io/crates/cargo-testify) â çè§æä»¶æ´æ¹ãè¿è¡æµè¯å¹¶éè¿åå¥½çæä½ç³»ç»éç¥éç¥ç»æ
- [cargo-tree](https://github.com/sfackler/cargo-tree) â Cargo å­å½ä»¤ï¼ä»¥æ ç¶æ ¼å¼å¯è§å crate çä¾èµå³ç³»å¾
- [cargo-update](https://crates.io/crates/cargo-update) â ç¨äºæ£æ¥ååºç¨æ´æ°å·²å®è£çå¯æ§è¡æä»¶çè´§ç©å­å½ä»¤ 
- [cargo-watch](https://crates.io/crates/cargo-watch) â è´§ç©å¨æºæ´æ¹æ¶ç¼è¯é¡¹ç®çå®ç¨ç¨åº
- [liuchong/cargo-x](https://github.com/liuchong/cargo-x) ââä¸ä¸ªéå¸¸ç®åçç¬¬ä¸æ¹ cargo å­å½ä»¤æ¥æ§è¡èªå®ä¹å½ä»¤
- [dtolnay/cargo-expand](https://github.com/dtolnay/cargo-expand) â æ©å±æºä»£ç ä¸­çå®
- [Devolutions/CMakeRust](https://github.com/Devolutions/CMakeRust) â ç¨äºå° Rust åºéæå° CMake é¡¹ç®ä¸­
- [SiegeLord/RustCMake](https://github.com/SiegeLord/RustCMake) â ä¸ä¸ªç¤ºä¾é¡¹ç®ï¼å±ç¤ºäº CMake ä¸ Rust çä½¿ç¨ 
- [icepuma/rust-action](https://github.com/icepuma/rust-action) ââRust github å¨ä½
- [peaceiris/actions-mdbook](https://github.com/peaceiris/actions-mdbook) â mdBook ç GitHub æä½
- GitHub ç½ç»é©å­
- [snare](https://tratt.net/laurie/src/snare/) â GitHub webhooks è¿è¡å¨å®æ¤è¿ç¨
- ç½ç»å
- [mxseev/rust-loader](https://github.com/mxseev/rust-loader) â Webpack Rust å è½½å¨ (wasm)

### è°è¯

- [rust-gdb](https://github.com/rust-lang/rust/blob/master/src/etc/rust-gdb)
- [gdbgui](https://github.com/cs01/gdbgui) â åºäºæµè§å¨ç gdb åç«¯ï¼ç¨äºè°è¯ CãC++ãRust å Go.
- [lldb_batchmode.py](https://github.com/rust-lang/rust/blob/master/src/etc/lldb_batchmode.py) â åè®¸ä»¥ç±»ä¼¼äº GDB çæ¹å¤çæ¨¡å¼çæ¹å¼ä½¿ç¨ LLDB.
- [CodeLLDB](https://marketplace.visualstudio.com/items?itemName=vadimcn.vscode-lldb) â ä¸ä¸ª LLDB æ©å± [Visual Studio Code](https://code.visualstudio.com/).

### é¨ç½²

- [emk/rust-musl-builder](https://github.com/emk/rust-musl-builder) â ç¨äºä½¿ç¨ musl-libc å musl-gcc ç¼è¯éæ Rust äºè¿å¶æä»¶ç Docker æ åï¼ä»¥åæç¨ç C åºçéæçæ¬
- [kpcyrd/mini-docker-rust](https://github.com/kpcyrd/mini-docker-rust) â ä¸ä¸ªéå¸¸å°ç Rust docker éåçç¤ºä¾é¡¹ç® 
- [liuchong/docker-rustup](https://github.com/liuchong/docker-rustup) â å¤çæ¬ï¼ä½¿ç¨ musl å·¥å·ï¼Rust Docker éå
- [messense/rust-musl-cross](https://github.com/messense/rust-musl-cross) â ä½¿ç¨ musl-cross ç¼è¯éæ Rust äºè¿å¶æä»¶ç Docker éå 
- [rust-lang-nursery/docker-rust](https://github.com/rust-lang/docker-rust) â å®æ¹ Rust Docker éå
- [wasm-template-rust](https://github.com/sn99/wasm-template-rust) â Rust åå¸å° gh-pages ç wasm æ¨¡æ¿ï¼æ é npm-deploy 
- [DenisKolodin/rust-app-engine](https://github.com/DenisKolodin/rust-app-engine) â App Engine Rust æ ·æ¿
- [emk/heroku-buildpack-rust](https://github.com/emk/heroku-buildpack-rust) â Heroku ä¸ç Rust åºç¨ç¨åºæå»ºå

### åµå¥å¼

- [japaric/rust-cross](https://github.com/japaric/rust-cross) ââå³äºäº¤åç¼è¯ Rust ç¨åºä½ éè¦ç¥éçä¸å
- [japaric/xargo](https://github.com/japaric/xargo) â è½»æ¾å°å° Rust ç¨åºäº¤åç¼è¯å°èªå®ä¹çè£¸æºç®æ ï¼å¦ ARM Cortex-M
- [Ogeon/rust-on-raspberry-pi](https://github.com/Ogeon/rust-on-raspberry-pi) â æå³å¦ä½ä¸º Raspberry Pi äº¤åç¼è¯ Rust é¡¹ç®çè¯´æ. * é¿æè¯º
- [avr-rust/ruduino](https://github.com/avr-rust/ruduino) `t Arduino Uno çå¯éç¨ç»ä»¶.

### FFI

ä¹å¯ä»¥çç [Foreign Function Interface](https://doc.rust-lang.org/book/first-edition/ffi.html), [The Rust FFI Omnibus](http://jakegoulding.com/rust-ffi-omnibus/) ï¼ä½¿ç¨å¶ä»è¯­è¨ç¨ Rust ç¼åçä»£ç çç¤ºä¾éåï¼å [FFI examples written in Rust](https://github.com/alexcrichton/rust-ffi-examples).

- [rlhunt/cbindgen](https://github.com/eqrion/cbindgen) â ä» Rust æºæä»¶çæ C å¤´æä»¶. å¨ Gecko ä¸­ç¨äº WebRender 
- [Sean1708/rusty-cheddar](https://github.com/Sean1708/rusty-cheddar) â ä» Rust æºæä»¶çæ C å¤´æä»¶
- [rust-lang/rust-bindgen](https://github.com/rust-lang/rust-bindgen) â Rust ç»å®çæå¨
- [dtolnay/cxx](https://github.com/dtolnay/cxx) â Rust å C++ ä¹é´çå®å¨äºæä½
- [rust-cpp](https://crates.io/crates/cpp) - ç´æ¥å¨ Rust ä¸­åµå¥ C++ ä»£ç 
- [rusterlium/rustler](https://github.com/rusterlium/rustler) â ç¨äºåå»º Erlang NIF å½æ°çå®å¨ Rust æ¡¥ 
- [mgattozzi/curryrs](https://github.com/mgattozzi/curryrs) â å¼¥å Haskell å Rust ä¹é´çå·®è·
- [mgattozzi/haskellrs](https://github.com/mgattozzi/haskellrs) â Haskell FFI ç¤ºä¾ä¸­ç Rust
- [mgattozzi/rushs](https://github.com/mgattozzi/rushs) â Rust FFI ç¤ºä¾ä¸­ç Haskell
- [j4rs](https://crates.io/crates/j4rs) â ä½¿ç¨ Rust ä¸­ç Java 
- [bennettanderson/rjni](https://github.com/benanders/rjni) â ä½¿ç¨ Rust ä¸­ç Java
- [drrb/java-rust-example](https://github.com/drrb/java-rust-example) â ä½¿ç¨ Java ä¸­ç Rust
- [jni](https://crates.io/crates/jni) â ä½¿ç¨ Java ä¸­ç Rust
- [jni-sys](https://crates.io/crates/jni-sys) â å¯¹åºäº jni.h ç Rust å®ä¹ 
- [rucaja](https://crates.io/crates/rucaja) â ä½¿ç¨ Rust ä¸­ç Java 
- [rawrafox/rust-jdbc](https://github.com/rawrafox/rust-jdbc) â ä½¿ç¨æ¥èª Rust ç JDBC
- [jcmoyer/rust-lua53](https://github.com/jcmoyer/rust-lua53) â ç¨äº Rust ç Lua 5.3 ç»å®
- [lilyball/rust-lua](https://github.com/lilyball/rust-lua) â Safe Rust bindings to Lua 5.1
- [tickbh/td_rlua](https://github.com/tickbh/td_rlua) â Rust çé¶ææ¬é«çº§ lua 5.3 åè£å¨
- [tomaka/hlua](https://github.com/tomaka/hlua) - ä¸ Lua äº¤äºç Rust åº 
- [anima-engine/mrusty](https://github.com/anima-engine/mrusty) â Rust ç mruby å®å¨ç»å®
- [neon-bindings/neon](https://github.com/neon-bindings/neon) â Rust ç»å®ï¼ç¨äºç¼åå®å¨ä¸å¿«éçåç Node.js æ¨¡å
- [infinyon/node-bindgen](https://github.com/infinyon/node-bindgen) - ä½¿ç¨ Rust çæ nodejs æ¨¡åçç®åæ¹æ³ * ç®æ  - C
- [SSheldon/rust-objc](https://github.com/SSheldon/rust-objc) â Rust ç Objective-C è¿è¡æ¶ç»å®ååè£å¨
- [vickenty/mi-rust](https://github.com/vickenty/mi-rust) â æ·»å å¯¹ M::I çæ¯æï¼ä»¥ä½¿ç¨ Cargo æå»ºæ¨¡å
- [vickenty/perl-xs](https://github.com/vickenty/perl-xs) â ä½¿ç¨ Rust åå»º Perl XS æ¨¡å 
- [getsentry/milksnake](https://github.com/getsentry/milksnake) â python setuptools çæ©å±ï¼å®åè®¸æ¨ä»¥å¯æ³è±¡çæä¾¿æºçæ¹å¼å¨ Python è½®å­ä¸­ååå¨æé¾æ¥åº.
- [dgrunwald/rust-cpython](https://github.com/dgrunwald/rust-cpython) â Python ç»å®
- [PyO3/PyO3](https://github.com/PyO3/PyO3) â Python è§£éå¨ç Rust ç»å® 
- [d-unseductable/ruru](https://github.com/d-unseductable/ruru) â ç¨ Rust ç¼åçåç Ruby æ©å± 
- [danielpclark/rutie](https://github.com/danielpclark/rutie) â ç¨ Rust ç¼åçåç Ruby æ©å±ï¼åä¹äº¦ç¶ 
- [tildeio/helix](https://github.com/tildeio/helix) â ç¨ Rust ç¼å Ruby ç±» 
- [rustwasm/wasm-pack](https://github.com/rustwasm/wasm-pack) â   æå wasm å¹¶åå¸å° npmï¼
- [rustwasm/wasm-bindgen](https://github.com/rustwasm/wasm-bindgen) â ä¸ä¸ªä¿è¿ wasm æ¨¡åå JS ä¹é´é«çº§äº¤äºçé¡¹ç®. 
- [rhysd/wain](https://github.com/rhysd/wain) - wainï¼å¨ Safe Rust ä¸­ä»é¶å¼å§ç WebAssembly è§£éå¨ï¼é¶ä¾èµ 
  
### IDEs

ä¹å¯ä»¥çç [Are we (I)DE yet?](https://areweideyet.com/) å [Rust Tools](https://www.rust-lang.org/tools).

- Atom

  - [zargony/atom-language-rust](https://github.com/zargony/atom-language-rust)
  - [rust-lang/atom-ide-rust](https://github.com/rust-lang/atom-ide-rust) â Rust IDE å¯¹ Atom çæ¯æï¼ç± Rust è¯­è¨æå¡å¨ (RLS) æä¾æ¯æ

- Eclipse

  - [Eclipse Corrosion](https://github.com/eclipse/corrosion)
  - [RustDT](https://github.com/RustDT/RustDT) 

- Emacs

  - [rust-mode](https://github.com/rust-lang/rust-mode) â Rust ä¸»è¦æ¨¡å¼
  - [rustic](https://github.com/brotzeit/rustic) - Emacs ç Rust å¼åç¯å¢ 
  - [flycheck-rust](https://github.com/flycheck/flycheck-rust) â Rust æ¯æ [Flycheck](https://github.com/flycheck/flycheck)
  - [emacs-racer](https://github.com/racer-rust/emacs-racer) â èªå¨å®æï¼å¦è§ [company](https://company-mode.github.io/) å [auto-complete](https://github.com/auto-complete/auto-complete))

- [gitpod.io](https://gitpod.io/) â åºäº Rust è¯­è¨æå¡å¨çå·æå®æ´ Rust æ¯æçå¨çº¿ IDE

- [gnome-builder](https://wiki.gnome.org/Apps/Builder) èªçæ¬ 3.22.2 èµ·åçæ¯æ Rust å Cargo

- Kakoune

  - [kak-lsp/kak-lsp](https://github.com/kak-lsp/kak-lsp/) â [LSP](https://microsoft.github.io/language-server-protocol/) å®¢æ·. å¨ Rust ä¸­å®ç°å¹¶æ¯æ rls å¼ç®±å³ç¨.

- NetBeans

  - [drrb/rust-netbeans](https://github.com/drrb/rust-netbeans)

- IntelliJ

  - [intellij-rust/intellij-rust](https://github.com/intellij-rust/intellij-rust) 
  - [intellij-rust/intellij-toml](https://github.com/intellij-rust/intellij-toml) â åºæ¬ç Toml æ¯æ

- [Ride](https://github.com/madeso/ride)

- [SolidOak](https://github.com/oakes/SolidOak) â ä¸ä¸ªç®åç Rust IDEï¼åºäº GTK+ å [Neovim](https://github.com/neovim/neovim)

- Sublime Text

  - [rust-lang/rust-enhanced](https://github.com/rust-lang/rust-enhanced) â å®æ¹ Rust å
  - [sublimehq/packages](https://github.com/sublimehq/Packages/tree/master/Rust) â åç Sublime æ¯æï¼å·²å®è£ï¼

- Vim

  â æ å¤ä¸å¨çææ¬ç¼è¾å¨

  - [rust.vim](https://github.com/rust-lang/rust.vim) â æä¾æä»¶æ£æµãè¯­æ³é«äº®ãæ ¼å¼åãSyntastic éæç­.
  - [vim-cargo](https://github.com/timonv/vim-cargo) â å½ä»¤ç»å®ä»¥ä» vim å¿«éè¿è¡è´§ç©.
  - [vim-racer](https://github.com/racer-rust/vim-racer) â åè®¸ vim ä½¿ç¨ [Racer](https://github.com/racer-rust/racer) ç¨äº Rust ä»£ç å®æåå¯¼èª.
  - [autozimu/LanguageClient-neovim](https://github.com/autozimu/LanguageClient-neovim) â [LSP](https://microsoft.github.io/language-server-protocol/) å®¢æ·. å¨ Rust ä¸­å®ç°å¹¶æ¯æ rls å¼ç®±å³ç¨

- è§è§å·¥ä½å®¤

  - [PistonDevelopers/VisualRust](https://github.com/PistonDevelopers/VisualRust) â Rust ç Visual Studio æ©å±
  - [dgriffen/rls-vs2017](https://github.com/ZoeyR/rls-vs2017) â å¯¹ Visual Studio 2017 é¢è§çç Rust æ¯æ

- Visual Studio Code

  - [rust-lang/rls-vscode](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust) â å¯¹ Visual Studio Code ç Rust æ¯æ
  - [rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer) â RLS çæ¿ä»£ Rust è¯­è¨æå¡å¨
  - [CodeLLDB](https://marketplace.visualstudio.com/items?itemName=vadimcn.vscode-lldb) â ä¸ä¸ª LLDB æ©å±
  - [crates](https://github.com/serayuzgur/crates) â crates æ¯ crates.io ä¾èµé¡¹çæ©å±. 
  
### å¾åè¯å«

- [sfikas/rusteval](https://github.com/sfikas/rusteval) â ç¨äºè¯ä¼°æ£ç´¢ç®æ³è¾åºçå·¥å· 

### åæ

- [bheisler/criterion.rs](https://github.com/bheisler/criterion.rs) â ç»è®¡é©±å¨ç Rust åºåæµè¯åº
- [sharkdp/hyperfine](https://github.com/sharkdp/hyperfine) â å½ä»¤è¡åºåæµè¯å·¥å· 
- [performancecopilot/hornet](https://github.com/performancecopilot/hornet) â Performance Co-Pilot åå­æ å°å¼æ£æµåº 
- [koute/memory-profiler](https://github.com/koute/memory-profiler) â Linux çåå­åæå¨ 
- [ellisonch/rust-stopwatch](https://github.com/ellisonch/rust-stopwatch) â ä¸ä¸ªç§è¡¨åº 
- [mrhooray/torch](https://github.com/mrhooray/torch) â æ ¹æ® DWARF è°è¯ä¿¡æ¯çæ FlameGraphs
- [llogiq/flame](https://github.com/llogiq/flame) 

### Services

- [deps.rs](https://github.com/deps-rs/deps.rs) â æ£æµè¿æ¶æä¸å®å¨çä¾èµé¡¹
- [docs.rs](https://docs.rs/) â èªå¨çæ crate ææ¡£
  
### éæåæ

- [facebookexperimental/MIRAI](https://github.com/facebookexperimental/mirai) â ä¸ä¸ªå¨ Rust çä¸­çº§ä¸­é´è¡¨ç¤º (MIR) ä¸è¿è¡çæ½è±¡è§£éå¨
- [static_assertions](https://crates.io/crates/static_assertions) â ç¼è¯æ¶æ­è¨ä»¥ç¡®ä¿æ»¡è¶³ä¸åé 

### æµè¯

- [laboratory](https://crates.io/crates/laboratory) â ä¸ä¸ªç®åãå¯æè¡¨ç°åç Rust ååæµè¯æ¡æ¶ 
- [cucumber-rust](https://crates.io/crates/cucumber-rust) â Rust ç Cucumber æµè¯æ¡æ¶çå®ç°.
- [demonstrate](https://crates.io/crates/demonstrate) â å£°æå¼æµè¯æ¡æ¶ 
- [httpmock](https://github.com/alexliesenfeld/httpmock) â HTTP æ¨¡æ 
- [mockiato](https://crates.io/crates/mockiato) â ä¸ä¸ªä¸¥æ ¼ä½åå¥½ç Rust 2018 æ¨¡æåº
- [mutagen](https://crates.io/crates/mutagen) â ä¸ä¸ªæºçº§åå¼æµè¯æ¡æ¶ï¼ä»éæ¯æï¼
- [AlKass/polish](https://github.com/AlKass/polish) â è¿·ä½ æµè¯ / æµè¯é©±å¨æ¡æ¶ 
- [proptest](https://crates.io/crates/proptest) â åå¯åçå±æ§æµè¯æ¡æ¶ [Hypothesis](https://hypothesis.works/) Python æ¡æ¶
- [quickcheck](https://crates.io/crates/quickcheck) â ä¸ä¸ª Rust å®ç° [QuickCheck](https://wiki.haskell.org/Introduction_to_QuickCheck1) 
- [mockito](https://crates.io/crates/mockito) â HTTP æ¨¡æ 
- [speculate](https://crates.io/crates/speculate) â ä¸ä¸ª RSpec å¯åäº Rust çæå°æµè¯æ¡æ¶
- [rstest](https://crates.io/crates/rstest) â Rust çåºäºå¤¹å·çæµè¯æ¡æ¶
- [ruspec](https://crates.io/crates/ruspec) â å Rspec æµè¯æ¡æ¶ä¸æ ·ç¨ Rust ç¼å 
- [rust-fuzz/afl.rs](https://github.com/rust-fuzz/afl.rs) â ä¸ä¸ª Rust æ¨¡ç³å¨ï¼ä½¿ç¨ [AFL](https://lcamtuf.coredump.cx/afl/) 
- [tarpaulin](https://crates.io/crates/cargo-tarpaulin) â ä¸º Rust è®¾è®¡çä»£ç è¦ççå·¥å· 
- [trust](https://github.com/japaric/trust) â Travis CI å AppVeyor æ¨¡æ¿ï¼ç¨äºå¨ 5 ç§æ¶æä¸æµè¯æ¨ç Rust crate å¹¶åå¸å¶éç¨äº LinuxãmacOS å Windows çäºè¿å¶çæ¬
- [fake-rs](https://github.com/cksac/fake-rs) â çæåæ°æ®çåº 
- [goldenfile](https://github.com/calder/rust-goldenfile) - ä¸ä¸ªä¸º Goldenfile æµè¯æä¾ç®å API çåº.
- [cargo-dinghy](https://crates.io/crates/cargo-dinghy/) - ç®åå¨æºè½ææºåå¶ä»å°åå¤çå¨è®¾å¤ä¸è¿è¡åºæµè¯åå·¥ä½å°çè´§ç©æ©å±.

### ç¿»è¯å¨

- [immunant/c2rust](https://github.com/immunant/c2rust) â å¨ Clang/LLVM ä¹ä¸æå»ºç C å° Rust ç¿»è¯å¨åäº¤åæ£æ¥å¨. 
- [jameysharp/corrode](https://github.com/jameysharp/corrode) â ç¨ Haskell ç¼åç AC å° Rust ç¿»è¯å¨.

## æ¶éç³»ç»ä¿¡æ¯

- [Phate6660/nixinfo](https://github.com/Phate6660/nixinfo) [[crate](https://crates.io/crates/nixinfo)] â ä¸ä¸ªç¨äºæ¶éç³»ç»ä¿¡æ¯ï¼å¦ CPUãåè¡çãç¯å¢ãåæ ¸ç­ï¼ç lib crate.
  
# ð å¤§çè¯­å½
  
### Matthieum:
  
âRust ä½¿ç¼åæ­£ç¡®ä¸å¯è¯»çä»£ç åå¾æ´å®¹æï¼åæ¶è·å¾ä¸¤èå¹¶éå·§åã

æææ/åç¨æºå¶ï¼å¯¹çå½å¨æãå«ååå¯åæ§çä¸¥æ ¼æ§å¶ï¼å¨çæçè½¯ä»¶çæ°æ®æµä¸­å¼ºå¶æ§è¡æç§ç®åæ§ï¼æ¨å¯ä»¥å¨å¶ä»ç¼ç¨è¯­è¨ä¸­è·å¾è¿ç§ç®åæ§ï¼ä½éå¸¸ä¸ä¼ï¼å ä¸ºè¯¥è¯­è¨æ´å®½æ¾ä½ å¾å°äºä¸ä¸ªæ´å¤æçæµç¨ã

ä½ æ¯å¦æ¾ç»å¨ Java ä¸­è°è¯è¿ ConcurrentModificationExceptionï¼å½æ¨ä¿®æ¹æ­£å¨è¿­ä»£çå®¹å¨æ¶ä¼åçè¿ç§æåµãå½æ¨æä¸ç³»ååè°/è§å¯èæ¶ï¼æå¤å°æå¯¼è´æ­¤å¼å¸¸çå¾ªç¯å¼ç¨éå¸¸å®¹æãå¨ Rust ä¸­ï¼è¦è§£å³è¿ç§æåµï¼ä½ å¿é¡»ä½¿ç¨ RefCell æç­ä»·ç©ï¼å®åºè¯¥è®©æ¨åä¸æ¥ãâ


## èç³»ä¸æ 

#### å³æ³¨å¾®ä¿¡å¬ä¼å·ãåå°æå¡æ¶æå¸ãââãèç³»æä»¬ãï¼è·åæ¬repoæå¨PDFå­¦ä¹ ææ¡£ï¼

<img width="65%" height="65%" src="https://user-images.githubusercontent.com/87457873/130796999-03af3f54-3719-47b4-8e41-2e762ab1c68b.png"/>
  
  
  
  
  
