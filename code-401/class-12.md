# Class 12 Reading Notes

## Socket.io

### Web Sockets

1. What is a Web Socket?

- computer communications protocol that is bidirectional and is compatible with HTTP.

2. Describe the Web Socket request/response handshake and what happens once the connection is established.

- The WebSocket authentication uses the HTTP upgrade header to change from an HTTP protocol to the WebsSocket protocol. This allows communication between the web browser and the server. The server sends content to the client without first being requested by the client and allows messaging back and forth while maintaining the connection.

3. Web Sockets provide a standardized way for the server to send content to a client without first receiving a _request___ from that client.


### Socket.io Tutorial

1. What does the event handler io.on() do?

- Adds a listener that will be fired when any event is emitted

2. Describe some possible proof of life or proof that the code works as expected

3. What does socket.emit() do?

- sends a message to all the connected clients that notifies when a user connects to the server.socket

### Socket.io vs Web Sockets

1. What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).

- WebSocket is a communication protocol that provides bidirectional communication between the client and the server. It remains open all the time and allows real-time data transfer. Socket.IO is a library that enables real-time communication between the client and the web servers that **uses** WebSocket protocol to provide the interface.

2. When would you use Socket.IO?

- Socket.IO is a library that allows two way communication that is built on top of WebSocket

3. When would you use WebSockets?

- WebSockets is used when you want two-way communication between two networked systems like an instant message platform.