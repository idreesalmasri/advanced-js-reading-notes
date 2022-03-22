## Review, Research, and Discussion
What does it mean that web sockets are bidirectional? Why is this useful?

WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time.

Does socket.io use HTTP? Why?

WebSocket uses HTTP as the initial transport mechanism, but keeps the TCP connection alive after the HTTP response is received so that it can be used for sending messages between client and server. 

What happens when a client emits an event?
in the server threre are eventes listen and when client emites evente it will envok specifice function 

What happens when a server emits an event?
the server will send response for all clientes connected to the server 

### Terms
Socket:
A socket is one endpoint of a two-way communication link between two programs running on the network. 

Web Socket:
a persistent connection between a client and server. WebSockets provide a bidirectional, full-duplex communications channel that operates over HTTP through a single TCP/IP socket connection.
Socket.io:
Socket.IO is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, and a server-side library for Node.js.
Server:
a computer or system that provides resources, data, services, or programs to other computers, known as clients, over a network.
TCP Model:
TCP/IP Reference Model is a four-layered suite of communication protocols.
UDP:
User Datagram Protocol (UDP) is a communications protocol that is primarily used to establish low-latency and loss-tolerating connections between applications on the internet.