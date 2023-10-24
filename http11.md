# HTTP1.1

**What is HTTP?**
HTTP stands for _The Hypertext Transfer Protocol_ which is the foundation of the WWW, _World Wide Web_, and is an application-level protocol for distributed, collaborative, hypermedia information systems. The protocol was designed to transfer information between networked devices and runs on top of other layers of the network.
A typical flow over HTTP involves a client machine making a request to a server,which then sends a response message.

**What is HTTP1.1 and what makes it different from over versions?**
HTTP1.1 is the first usable version of http created in 1997.
The first version of HTTP, referred to as HTTP0.9 was a simplke protocol for raw data transfer across the internet.
HTTP1.1 includes more stringent requirement to ensure reliable implemetation of its features.
This includes cache controls and content negotiation that allowed for different languages, content encodings, and types.
HTTP1.1 is still used on the web.

HTTP1.1 flow control replies on the underlying TCP, _transport layer_ connection. This avoid buffer overflow. Each new TCP connection requires a separate flow control mechanism.
With persistent connections, HTTP1.1 assumes the TCP connection should be kept open unless directyly told to close which allows the client. This allows client to send multiplek requests along the same connectionw ithout waiting for a response to each.
HTTP2 is the reimagined version in 2015 which offered several methods to decrease latency.
HTTP2 multplexes streams within a single TCP connection however, because of this recieve windows on the level of the TCP connection are not sufficient to regulate the delivery of individual streams.
