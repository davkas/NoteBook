###Netty综述
------

####1. Netty架构
------
#####传输服务（Transport Service）
- Socket & Datagram
- HTTP Tunnel
- In-VM Pipe
#####协议支持（rotocol Support）
------
- HTTP&WebSocket
- SSL StartTLS
- Google Protobuf
- zlib/gzip Compression
- Large File Transfer
- RTSP
- Legacy Text、Binary Protocols with Unit Testability
#####核心功能（Core）
------
- Extensible Event Model
- Universal Communication API
- Zero-Copy-Capable Rich Byte Buffer

####2. Netty服务器端流程
------
#####一个Netty服务器程序的构建主要由两部分组成：
- 配置服务器的功能，如线程，端口等
- 实现服务器处理程序，它包含业务逻辑，决定当有一个请求连接或接受数据时的处理逻辑
#####使用Netty编写服务器程序的实现的过程如下：
- 创建ServerBootstrap实例引导绑定和启动服务器
- 创建NioEventLoopGroup对象来处理事件，如接受新连接、接受数据、写数据等。
- 制定InetSocketAddress，服务器监听此端口
- 设置childHandler执行所有的连接请求
- 调用ServerBootStrap.bind()方法绑定服务器
- 编写Handler的实例类完成业务逻辑的处理


####3. Netty客户端流程
------
####4. Netty中关于“著名的epoll缺陷”

####5.Netty中的核心概念




