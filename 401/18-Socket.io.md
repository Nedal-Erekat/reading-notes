# Socket.io
WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.
> WebSocket is distinct from HTTP. Both protocols are located at layer 5 in the OSI model and depend on TCP at layer 4.
> To achieve compatibility, the WebSocket handshake uses the HTTP Upgrade header[1] to change from the HTTP protocol to the WebSocket protocol.

## Key features of WebSocket 

WebSocket helps in real-time communication between the Client and the web server.
This protocol helps in transforming to cross-platform in a real time world between the server and the client.
This also enables the business around the world for real-time web application to enhance and to increase the feasibility.
The major advantage it stands over an HTTP connection that it provides full duplex communication

## Key features of Socket.IO
It helps in broadcasting to multiple sockets at a time and handles the connection transparently.
It works on all platform, server or device ensuring the equality, reliability, and speed.
It automatically upgrades the requirement to WebSocket if needed.
It is a custom real-time transport protocol implementation on top of other protocols.
It requires both libraries to be used Client side as well as a server-side library.
IO works on work-based events. there are some reserved events which can be accessed using the Socket on server side like Connect, message, Disconnect, Ping and Reconnect.
There are some Client based reserved events like Connect, connect- error, connect-timeout and Reconnect etc.

## Difference Between WebSocket and Socket.io

> WebSocket is technology while Socket.io is a library for WebSockets.

WebSocket is the communication Protocol which provides bidirectional communication between the Client and the Server over a TCP connection, WebSocket remains open all the time so they allow the real-time data transfer. When clients trigger the request to the Server it does not close the connection on receiving the response, it rather persists and waits for Client or server to terminate the request.

Socket.IO is a library which enables real-time and full duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts, both WebSocket vs Socket.io are event-driven libraries

Client Side: it is the library that runs inside the browser
Server Side: It is the library for Node.js