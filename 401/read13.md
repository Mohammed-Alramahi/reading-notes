# Message Queues

## What does it mean that web sockets are bidirectional? Why is this useful?

* it means communication goes in two directions between client and server.

* this is useful because a conversation can be kept going between a server and client

## Does socket.io use HTTP? Why?

Yes. Socket.io servers attach to HTTP servers to communication with clients.

## What happens when a client emits an event?

The client emits an event and then the server handles the event using the on method.

## What happens when a server emits an event?

The server emits an event and then the client that the event was emitted to handles the event.

## What happens if a client “misses” an event?

Nothing. The event will be ignored if it is missed.

## How can we mitigate this?

We could assign unique IDs to events in order to track them, log events, and make sure the client recieved the event.

## Document the following Vocabulary Terms

### Socket

an endpoint for the transmission of data

### Web Socket

A communication protocol for establishing a connection for servers and clients to transmit data

### Socket.io

A javascript library for realtime, bi-directional communication between servers and clients

### Client

Accesses services or functionality from server

### Server

Provides services and functionality for clients

### OSI Model

Open Systems Interconnection Model:

Physical Layer -> Data Link Layer -> Network Layer -> Transport Layer -> Session Layer -> Presentation Layer -> Application Layer

### TCP Model

Transmission Control Protocol Model:

Network Access Layer -> Internet Layer -> Transport Layer -> Application Layer

### TCP

Transmission Control Protocol - a connection-based communication protocol used for the transmission of data within a network.

### UDP

The User Datagram Protocol - a communication protocol used for time-sensitive transmission of data. Like real time applications.

### Packets

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

TCP, OSI model, web sockets

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

Socket io on client side, using socket io with an api, events broadcast.

### What are you most excited about trying to implement or see how it works?

A real-time chatroom or messaging queue

### Chat

Sockets have traditionally been the solution around which most real-time chat systems are architected, providing a bi-directional communication channel between a client and a server.

This means that the server can push messages to clients. Whenever you write a chat message, the idea is that the server will get it and push it to all other connected clients.

### Rooms

A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients

## Resources

[Socket.io Chat Example](https://socket.io/get-started/chat/)

[Rooms and Namespaces](https://socket.io/docs/rooms-and-namespaces/)

[Socket.io Emit Cheatsheet](https://socket.io/docs/emit-cheatsheet/)