# Rooms
Within each Namespace, you can define arbitrary channels called “Rooms” that sockets can join and leave.
This is useful to broadcast data to a subset of sockets:

## Joining and leaving
can call join to subscribe the socket to a given channel,And then simply use to or in (they are the same) when broadcasting or emitting,You can emit to several rooms at the same time:

- You can also broadcast to a room from a given socket.


# Review:


What does it mean that web sockets are bidirectional? Why is this useful?
- full duplex communication between the Client and the Web servers.

Does socket.io use HTTP? Why?
- Even when websockets can be used, the initial connection setup it done over HTTP. Also, a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js

What happens when a client emits an event?
- it will trigger the event that is listening in the server

What happens when a server emits an event?
- it depend we can make specific client of all client listen to it


* Web Socket: s the communication Protocol which provides bidirectional communication between the Client and the Server over a TCP connection, 
* Socket.IO is a library which enables real-time and full duplex communication between the Client and the Web servers. 
