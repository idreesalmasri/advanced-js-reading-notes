## Socket.io
Review, Research, and Discussion (Links to an external site.)
1- What is the benefit of transforming data into packets?

enable new innovations, services, and business opportunities.

2- UDP is often refereed to as a connectionless protocol. Why is this?

because it is analogous to sending a letter where you don’t acknowledge receipt.

3- Can a socket server application have multiple socket connections?

Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs,

4- Can a socket connection application be connected to multiple socket servers?

You cannot use a single socket to connect to multiple servers. You must create a separate socket for each connection.

4- Can an application be both a socket server and a socket connection?

You can use the same socket for whatever you want, as long as your protocol handles it.


Term 
Observer Pattern: The observer pattern is a software design pattern in which a subject object keeps track of its dependents, called observers, and notifies them of any state changes automatically, usually by calling one of their methods.

Listener: represents a handler for an event emitted by an EventTarget object.

Event Handler: is an asynchronous callback routine that runs after an event occurs.

Event Driven Programming: is utilized to make the program as easy as feasible by synchronizing the occurrence of various events.

Emit: (On the other hand, the publish method allows you to “emit” an event, causing any callbacks associated with the event to ‘fire’) (get called).

Event Loop: The event loop is a programming component or design pattern in which a program waits for and dispatches events or messages.

Event Queue: is a storage location for events from an application before they are processed by a receiving program or system.


Trigger: For the selected items, the trigger() method activates the provided event and the default behavior of an event (such as form submission).

Subscribe: The.subscribe() function is similar to jQuery’s Promise.then(),.catch(), and.finally() methods, but it works with Observables instead of promises.

Raise: raise an error,The throw statement throws a user-defined exception.

database: a structured collection of information or data that is usually saved electronically in a computer system.


Why Socket.IO?
Writing a real-time application with popular web applications stacks like LAMP (PHP) has traditionally been very hard. It involves polling the server for changes, keeping track of timestamps, and it is a lot slower than it should be.

Sockets have traditionally been the solution around which most real-time systems are architected, providing a bi-directional communication channel between a client and a server. This means that the server can push messages to clients. Whenever an event occurs, the idea is that the server will get it and push it to the concerned connected clients.

Socket.IO is quite popular, it is used by Microsoft Office, Yammer, Zendesk, Trello,. and numerous other organizations to build robust real-time systems. It one of the most powerful JavaScript frameworks on GitHub, and most depended-upon NPM (Node Package Manager) module. Socket.IO also has a huge community, which means finding help is quite easy.

WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

WebSocket is distinct from HTTP. Both protocols are located at layer 7 in the OSI model and depend on TCP at layer 4. Although they are different, RFC 6455 states that WebSocket "is designed to work over HTTP ports 443 and 80 as well as to support HTTP proxies and intermediaries", thus making it compatible with HTTP. To achieve compatibility, the WebSocket handshake uses the HTTP Upgrade header to change from the HTTP protocol to the WebSocket protocol.


