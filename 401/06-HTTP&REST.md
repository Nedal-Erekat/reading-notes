# HTTP and REST

- HTTP stands for Hypertext Transfer Protocol. It's a stateless, application-layer protocol for communicating between distributed systems, and is the foundation of the modern web. As a web developer, we all must have a strong understanding of this protocol.

- HTTP allows for communication between a variety of hosts and clients, and supports a mixture of network configurations.

> To make this possible, it assumes very little about a particular system, and does not keep state between different message exchanges.

* Communication between a host and a client occurs, via a request/response pair. The client initiates an HTTP request message, which is serviced through

### URLs
At the heart of web communications is the request message, which are sent via Uniform Resource Locators (URLs). I'm sure you are already familiar with URLs, but for completeness sake, I'll include it here. URLs have a simple structure that consists of the following components:

![](https://cdn.tutsplus.com/net/authors/jeremymcpeak/http1-url-structure.png)


#### There are some lesser used verbs that HTTP also supports:

- HEAD: this is similar to GET, but without the message body. It's used to retrieve the server headers for a particular resource, generally to check if the resource has changed, via timestamps.
- TRACE: used to retrieve the hops that a request takes to round trip from the server. Each intermediate proxy or gateway would inject its IP or DNS name into the Via header field. This can be used for diagnostic purposes.
- OPTIONS: used to retrieve the server capabilities. On the client-side, it can be used to modify the request based on what the server can support.

## Status Codes
With URLs and verbs, the client can initiate requests to the server. In return, the server responds with status codes and message payloads. The status code is important and tells the client how to interpret the server response. The HTTP spec defines certain number ranges for specific types of responses:
1. Informational Messages
2. Successful
3. Redirection
4. Client Error
5. Server Error

![](https://cdn.tutsplus.com/net/authors/jeremymcpeak/http1-req-res-details.png)

## What is REST
REST is acronym for REpresentational State Transfer
is a software architectural style that defines a set of constraints to be used for creating Web services. Web services that conform to the REST architectural style, called RESTful Web services
- RESTful Web services allow the requesting systems to access and manipulate textual representations of Web resources by using a uniform and predefined set of stateless operations