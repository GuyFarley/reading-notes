# Code 401 - Class 13 - Message Queues

## [Socket.io Chat Example](https://socket.io/get-started/chat/)

### Explain to a non-technical recruiter what the Chat Example (above) does

- This chat application uses express to create a server that the app will run on. Then Socket.IO is incorporated to handle the messages that are being sent back and forth

### What proof of life are we getting on the backend from the above app?

- When a new user connects to the app (as an incoming socket), it logs `a user connected` to the console

### Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?

`socket.broadcast.emit`

## [Rooms](https://socket.io/docs/v4/rooms)

### What is a room and how might a room be useful?

- A room is a separate channel that sockets can join or leave. This is useful when you want to broadcast events to a certain user or set of users, and not all users

### How do you join a room?

- the `join` method can be called to subscribe a socket to a room:

```
io.on("connection", (socket) => {
  socket.join("room name");
});
```

### how do you leave a room?

- Using the "disconnect" event:

```
io.on("connection", socket => {
  socket.on("disconnecting", () => {
    console.log(socket.rooms); // the Set contains at least the socket ID
  });

  socket.on("disconnect", () => {
    // socket.rooms.size === 0
  });
});
```

## [Namespaces](https://socket.io/docs/v4/namespaces/)

### What is a Namespace and what does it allow you to do?

- A namespace is a communication channel that allows you to "multiplex" (or split the logic of your app over a single shared connection)

### Each namespace potentially has its own what? (hint: 3 things)

- event handlers
- rooms
- middlewares

### Discuss a possible use case for separate namespaces

- Separate namespaces allow you to do things like create a channel that only authorized users have access to, or to create a custom channel per user

[Back to Home](../README.md)
