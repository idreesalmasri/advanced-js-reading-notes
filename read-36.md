##  Application State with Redux

What is Redux?
Redux is a predictable state container for JavaScript apps.
Redux takes away some of the hassles faced with state management in large applications. It provides you with a great developer experience, and makes sure that the testability of your app isn’t sacrificed for any of those.
As you develop React applications, you may find that keeping all your state in a top-level component is no longer sufficient for you.

You may also have a lot of data changing in your application over time.
Redux helps solve these kinds of problems. Mind you, it isn’t the only solution out there.

why using redux? 

Redux simply provides a subscription mechanism which can be used by any other code. That said, it is most useful when combined with a declarative view implementation that can infer the UI updates from the state changes, such as React or one of the similar libraries available.

What is state management in Redux?
State management is essentially a way to facilitate communication and sharing of data across components. It creates a tangible data structure to represent the state of your app that you can read from and write to. That way, you can see otherwise invisible states while you’re working with them.

How Redux works?
The way Redux works is simple. There is a central store that holds the entire state of the application. Each component can access the stored state without having to send down props from one component to another.

There are three building parts: actions, store, and reducers. Let’s briefly discuss what each of them does. This is important because they help you understand the benefits of Redux and how it’s to be used. We’ll be implementing a similar example to the login component above but this time in Redux.

Actions in Redux
Simply put, actions are events. They are the only way you can send data from your application to your Redux store. The data can be from user interactions, API calls, or even form submissions.

Actions are sent using the store.dispatch() method. Actions are plain JavaScript objects, and they must have a type property to indicate the type of action to be carried out. They must also have a payload that contains the information that should be worked on by the action. Actions are created via an action creator.

Reducers in Redux
Reducers are pure functions that take the current state of an application, perform an action, and return a new state. These states are stored as objects, and they specify how the state of an application changes in response to an action sent to the store.

It is based on the reduce function in JavaScript, where a single value is calculated from multiple values after a callback function has been carried out.


#### advantage of all Redux has to offer.
1- Performance Benefits  
React Redux implements many performance optimizations internally so that your own connected component only rerenders when it actually needs to.  
2- Ease of testing  
It is easy to test Redux apps since functions used to change the state of pure functions.  
3- State persistence  
You can persist some of the app’s state to local storage and restore it after a refresh. This can be really nifty.
4- Server-side rendering  
