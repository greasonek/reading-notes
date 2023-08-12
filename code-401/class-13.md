# Class 13 Reading Notes

## Message Queues

### Socket.io Chat Example

1. Explain to a non-technical recruiter what the Chat Example (above) does.

- The messaging example creates a Node.JS app using the express framework to create a single page web app that uses Socket.io to send messages and broadcast the event to the app, meaning the app uses an event listener that listens for and emits any event.

2. What proof of life are we getting on the backend from the above app?

- listening on *:3000

3. Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?

- Use the broadcast flag for emitting that socket. (ex) socket.broadcast.emit('hi');

### Rooms

1. What is a room and how might a room be useful?

- A room is a channel that sockets can join and leave and can be used to broadcast events to a subset of clients.

2. How do you join a room?

- Use join to subscribe a socket to a room. (io.on('connection',(socket)=> socket.join('some room))); and use to or in when emitting (io.to('some room').emit('some event')); can join several rooms at the same time (io.to("room1").to("room2").to("room3").to("room4").emit('some event'));

3. how do you leave a room?

- To leave a channel it is exactly like join except use 'leave'. Sockets will leave all the channels automatically. 

### Namespaces

1. What is a Namespace and what does it allow you to do?

- A namespace is a communication channel that allows you to split the logic of the app over a shared connection.

2. Each namespace potentially has its own what? (hint: 3 things)

- Event handlers, rooms and middlewares.

3. Discuss a possible use case for separate namespaces

- Creating separate namespaces allows authorized users to have specific logic that is separate from the rest of the app. For example, the admin has access to the event for deleting a user while other users would not have the access to that event.