# HTTP 

**HTTP** stands for *Hyper Text Transfer Protocol*.
HTTP allows for communication between a variety of hosts and clients, and supports a mixture of network configurations.
`
To make this possible, it assumes very little about a particular system, and does not keep state between different message exchanges.
`
This makes HTTP a stateless protocol. The communication usually takes place over TCP/IP, but any reliable transport can be used. The default port for TCP/IP is 80, but other ports can also be used. 
`Custom headers can also be created and sent by the client.`
Communication between a host and a client occurs, via a request/response pair. The client initiates an HTTP request message, which is serviced through a HTTP response message in return. We will look at this fundamental message-pair in the next section.


The current version of the protocol is HTTP/1.1, which adds a few extra features to the previous 1.0 version. The most important of these, in my opinion, includes persistent connections, chunked transfer-coding and fine-grained caching headers. We'll briefly touch upon these features in this article; in-depth coverage will be provided in part two.
## HTTP Verbs
__GET, POST, PUT,DELETE,HEAD, TRACE,OPTIONS__
URLs reveal the identity of the particular host with which we want to communicate, but the action that should be performed on the host is specified via HTTP verbs. Of course, there are several actions that a client would like the host to perform. HTTP has formalized on a few that capture the essentials that are universally applicable for all kinds of applications.

## HTTP Status Codes
* 100 Continue. The client SHOULD continue with its request
* 200 OK. The request has succeeded
* 203 Non-Authoritative Information
* 206 Partial Content
* 300 Multiple Choices
* 303 See Other
* 306 (Unused) 
* 400 Bad Request.
##  Using HTTP Methods for RESTful Services
The HTTP verbs comprise a major portion of our “uniform interface” constraint and provide us the action counterpart to the noun-based resource. The primary or most-commonly-used HTTP verbs (or methods, as they are properly called) are POST, GET, PUT, PATCH, and DELETE. These correspond to create, read, update, and delete (or CRUD) operations, respectively. There are a number of other verbs, too, but are utilized less frequently. Of those less-frequent methods, OPTIONS and HEAD are used more often than others.

