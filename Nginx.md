#### Nginx

##### 解释一下什么是Nginx?有什么特性？

Nginx 是一个Web服务器和反向代理服务器，用于Http、Https、SMTP、POP3 和 IMAP协议

特性包括：反向代理/L7负载均衡器、切入式Perl解释器、动态二进制升级、可用于重新编写URL,具有非常好的PCRE支持



##### 请解释Nginx如何处理HTTP请求

Nginx使用反应器模式，主事件循环等待操作系统发出准备事件的信号，这样数据就可以从套接字读取，在该实例中读取到缓冲区并进行处理，单个线程可以提供数万个并发连接

