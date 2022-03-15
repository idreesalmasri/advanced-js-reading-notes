## Review, Research, and Discussion
Why is access control important?
because it is a valuable security technique that can be used to regulate who or what can view or use any given resource. 

What is a role used for?
control access to areas and features within the Professional Archive Platform.

### terms
Authentication & Authorization:
authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to

Role Based Access Control:
is a mechanism that restricts system access to users using their roles and privileges and permissions.

## Event-Driven Programming in Node.js
Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision. 
example of Event-Driven Programming is The Web Browser.

Every time you interact with a webpage through it’s user interface, an event is happening. When you click a button a click event is triggered. When you press a key a keydown event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way.

Event-Driven Programming makes use of the following concepts:
- An Event Handler is a callback function that will be called when an event is triggered.
- A Main Loop listens for event triggers and calls the associated event handler for that event.

### EventEmitter
Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. 

there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.


We access the EventEmitter class through the events module. Once imported we’ll need to create a new object from the class to start using it.
```
const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter;
```

### Removing Listeners
To remove event listeners in EventEmitter we can use the removeListener or removeAllListeners method.
