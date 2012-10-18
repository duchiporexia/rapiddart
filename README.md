rapiddart
=========

tcp server, http server, websocket server. use coroutine , pthread and zeromq to promote concurrency performances.<br/>
TODO:<br/>
1. 多个线程监听不同端口，在同一线程中，启动多个协程处理不同的socket连接。<br/>
2. 加入超时调度器，采用最小堆。<br/>
3. 加入zeromq，从而把每个socket连接的请求转发给后端zeromq worker处理，在把结果返回给对应的socket。<br/>
4. 在主线程中监听/接受socket请求，然后重新分配给客户端连接端口，客户端做二次连接。从而客户端只需要记住一个连接端口。<br/>
5. 加入http请求解析，实现开放服务。<br/>
6. 加入websocket，支持服务器push技术，从而支持高性能的网页应用程序。<br/>
