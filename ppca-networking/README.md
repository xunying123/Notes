## 项目介绍

了解计算机网络的基本组成，了解相关协议，设计并实现一个简易的网络代理



## 注意事项

- PPCA并不是一个为了卷而设立的项目，在这里只要你遵循最基本的规定，完成必要的任务，你就完全不需要担心你的分数
- 因此希望大家是真的选择了自己感兴趣的项目，而不是为了分数在做东西。
- 祝大家玩的开心。

## 项目要求

基础要求: [简单socks5代理服务器](socks5.md)

任选实现：

- 透明代理
- 分流规则
  - 按ip分流
  - HTTP/TLS分流
  - 按程序分流
- 多级代理
- UDP代理
- TLS劫持
- HTTP捕获/修改/重放
- 反向代理
- Anything else

第一周要求实现完成基础任务，后面三周中完成合适数量的自选任务。

自选任务分值助教还在调整中。

有任何你想自己实现的功能都可以向助教申请，在助教评估其工作量之后会赋予其合适的分值。



## 评分标准

- 基础任务 25%
- 自选功能
  - 分数待定

有bonus



## 参考资料

**参考书**:

- [Beej’s Guide to Network Programming](https://beej.us/guide/bgnet/)
- [High Performance Browser Networking](https://hpbn.co/)
  - 书中内容远超出此次项目的要求, 只看 Networking 101 及 HTTP 中的一部分即可
  - [中文版 pdf](https://jbox.sjtu.edu.cn/l/O1voXQ)
- [TCP/IP Tutorial and Technical Overview](https://www.redbooks.ibm.com/redbooks/pdfs/gg243376.pdf)

**协议文档**:

- [RFC 1928: SOCKS Protocol Version 5](https://www.rfc-editor.org/rfc/rfc1928)
- [RFC 9293: Transmission Control Protocol (TCP)](https://www.rfc-editor.org/rfc/rfc9293)
- [RFC 768: User Datagram Protocol](https://www.rfc-editor.org/rfc/rfc768)
- [RFC 9112: HTTP/1.1](https://www.rfc-editor.org/rfc/rfc9112.html)
- [HTTP on MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP)
- [RFC 8446: The Transport Layer Security (TLS) Protocol Version 1.3](https://www.rfc-editor.org/rfc/rfc8446)

欢迎补充。



## 致谢

感谢2021级ACM班的梁亚伦为这个项目打下基础。