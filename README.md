# example_channel
example of Django channel project to implement WebSocket
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
