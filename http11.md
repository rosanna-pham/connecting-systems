# HTTP1.1

**What is HTTP1.1?**

HTTP1.1 is the first usable version of http created in 1997. 
HTTP stands for *The Hypertext Transfer Protocol* which is the foundation of the WWW, *World Wide Web*, and is used to load webpages using hypertext links.
The protocol was designed to transfer information between networked devices and runs on top of other layers of the network.
A typical flow over HTTP involves a client machine making a request to a server,which then sends a response message.
HTTP1.1 is still used on the web.

**What's the difference between HTTP1.1 and HTTP2?**

HTTP1.1 flow control replies on the underlying TCP, *transport layer* connection. This avoid buffer overflow. Each new TCP connection requires a separate flow control mechanism.
With persistent connections, HTTP1.1 assumes the TCP  connection should be kept open unless directyly told to close which allows the client. This allows client to send multiplek requests along the same connectionw ithout waiting for a response to each.
HTTP2 is the reimagined version in 2015 which offered several methods to decrease latency. 
HTTP2 multplexes streams within a single TCP connection however, because of this recieve windows on the level of the TCP connection are not sufficient to regulate the delivery of individual streams.
