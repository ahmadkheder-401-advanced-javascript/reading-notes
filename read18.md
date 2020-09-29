## WebSocket
WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

**Socket.IO** is a library that enables real-time, bidirectional and event-based communication between the browser and the server.

It consists of: 
        - node.js server
        - node.js client


**How does that work?**
The client will try to establish a WebSocket connection if possible, and will fall back on HTTP long polling if not.

### Terms:

- OSI Model: OSI stands for Open System Interconnection,it is a model provides a standard for different computer systems to be able to communicate with each other.

- TCP Model : stands for Transmission Control Protocol. it is model a version of the OSI model. It contains four layers, unlike seven layers in the OSI model. 

- TCP : Transmission Control Protocol,is a standard that defines how to establish and maintain a network conversation through which application programs can exchange data. 

- UDP : User Datagram Protoco, is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet.

- Packets : formatted unit carry the data in the protocols that the Internet uses

- Socket : is one endpoint of a two-way communication link between two programs running on the network,it is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to.