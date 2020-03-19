This is a sample project

project name: example_channel

simple demo project to show the usage of Django channels package
to implement the usage of WebSocket function

WebSocket protocl, which is defined in RFC6455, its propose and brief
introduction is listed as below:

The WebSocket Protocol is designed to supersede existing
   bidirectional communication technologies that use HTTP as a transport
   layer to benefit from existing infrastructure (proxies, filtering,
   authentication).  Such technologies were implemented as trade-offs
   between efficiency and reliability because HTTP was not initially
   meant to be used for bidirectional communication (see [RFC6202] for
   further discussion).  The WebSocket Protocol attempts to address the
   goals of existing bidirectional HTTP technologies in the context of
   the existing HTTP infrastructure; as such, it is designed to work
   over HTTP ports 80 and 443 as well as to support HTTP proxies and
   intermediaries, even if this implies some complexity specific to the
   current environment.  However, the design does not limit WebSocket to
   HTTP, and future implementations could use a simpler handshake over a

   dedicated port without reinventing the entire protocol.  This last
   point is important because the traffic patterns of interactive
   messaging do not closely match standard HTTP traffic and can induce
   unusual loads on some components.

WebSockets 101

正常情况下，Django使用HTTP请求实现客户端和服务器端的通信：

        客户端发送HTTP请求到服务器端
        Django解析请求，提取URL，并将其和view进行匹配
        view处理请求并返回HTTP Response至客户端
        不同于HTTP请求，WebSockets协议使用双向直接通信，也就是说不需要客户端发送请求，
服务器端就可以向发送数据。HTTP协议中，只有客户端可以发送请求和接收响应，WebSockets协议中，
服务器端可以同时与多个客户端进行通信。我们将使用ws://前缀而不是http://

