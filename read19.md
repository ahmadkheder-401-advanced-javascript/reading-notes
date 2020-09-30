# Message queuing

Message queuing allows applications to communicate by sending messages to each other. The message queue provides temporary message storage when the destination program is busy or not connected.

![](https://miro.medium.com/max/576/1*jyvAtVsULzry5eYG1QL3dw.png)

A **queue** is a line of things waiting to be handled, starting at the beginning of the line and processing it in sequential order. A message queue is a queue of messages sent between applications. It includes a sequence of work objects that are waiting to be processed.
A **message** is the data transported between the sender and the receiver application; it's essentially a byte array with some headers at the top. An example of a message could be something that tells one system to start processing a task, it could contain information about a finished task or just be a plain message.

## Terms
web Socket: The communication protocol that allows a client and a server to connect over a TCP protocol.
Socket.IO: is a library that enables real-time, bidirectional and event-based communication between the browser and the server.
Client: connected server that connect through another server.
server: the main srver  in the socketIO that enable communication with the client.