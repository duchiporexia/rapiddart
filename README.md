rapiddart
=========

tcp server, http server, websocket server. use callback , pthread and zeromq to promote concurrency performances.<br/>
TODO:<br/>
1. 多个线程监听不同端口，在同一线程中，启动多个协程处理不同的socket连接。<br/>
2. 加入zeromq，从而把每个socket连接的请求转发给后端zeromq worker处理，在把结果返回给对应的socket。<br/>
4. 加入http请求解析，实现开放服务。<br/>
5. 加入websocket，支持服务器push技术，从而支持高性能的网页在线应用程序。<br/>
