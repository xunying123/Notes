# 简单代理服务器

## 任务要求

实现一个 socks5 协议的简单代理服务器。只需支持 CMD CONNECT (建立 TCP 连接)，无需支持用户鉴权 (AUTH 只支持 0 即可)。

## 本地测试

建议使用浏览器插件 Proxy SwitchyOmega 将代理设置为你的代理服务器，设置后试图访问网络，观察代理服务器的流量。

可以在你的程序运行时输出流经的地址以辅助debug。

也可使用 `all_proxy` 环境变量在命令行中调试:

```sh
all_proxy=socks5h://localhost:8080 curl example.com
```

评测脚本会在本周稍晚时发布。

## 时间要求

暂定第二周周一前完成。

## 参考资料

[RFC 1928: SOCKS Protocol Version 5](https://www.rfc-editor.org/rfc/rfc1928)

