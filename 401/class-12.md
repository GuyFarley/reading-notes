# Code 401 - Class 12 - Socket.io

## [Web Sockets](https://en.wikipedia.org/wiki/WebSocket)

### What is a Web Socket?

- WebSocket is a communications protocol that provides full-duplex channels over a single TCP connection. It enables interaction between a client (like a web browser) and a server that is more efficient than other methods

### Describe the Web Socket request/response handshake and what happens once the connection is established

- WebSocket handshake uses the HTTP Upgrade header to change from HTTP protocol to WebSocket. Information can then be passed back and forth between client and server while keeping the connection open.

### Web Sockets provide a standardized way for the server to send content to a client without first receiving a **request** from that client

## [Socket.io Tutorial](https://www.tutorialspoint.com/socket.io/)

### What does the event handler io.on() do?

- Whenever someone connects to the server, `io.on()` gets executed. It's an event handler that handles connection, disconnection, etc. using the socket object.

### Describe some possible proof of life or proof that the code works as expected

- An example provided by [this tutorial](https://www.tutorialspoint.com/socket.io/) for proof of life would be:

```
<!DOCTYPE html>
<html>
   <head><title>Hello world</title></head>
   <script src="/socket.io/socket.io.js"></script>
   <script>
      var socket = io();
   </script>
   <body>Hello world</body>
</html>
```

### What does socket.emit() do?

- It emits events from the client

## [Socket.io vs Web Sockets](https://www.educba.com/websocket-vs-socket-io/)

### What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0)

- **WebSocket** is a communication Protocol that allows real-time data transfer (this would be like Git in the Git/GitHub comparison)
- **Socket.IO** is a library that uses WebSocket to provide an interface for enabling this real-time data transfer (this would be like GitHub in the Git/GitHub comparison)

### When would you use Socket.IO?

- To provide an interface for using WebSocket connections (it is a library that abstracts the connections)

### When would you use WebSockets?

- When it makes more sense to keep an open connection between client and server (for instance, with multiplayer gaming)

## [OSI Model Explained](https://www.youtube.com/watch?v=vv4y_uOneC0)

### What are a couple of key takeaways from this video?

## [TCP Handshakes Explained](https://www.youtube.com/watch?v=xMtP5ZB3wSk)

### Translate the gist of this video to a non-technical friend

[Back to Home](../README.md)
