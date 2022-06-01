## Redux - Asynchronous Actions
### Async Logic and Data Fetching
By itself, a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.  

A "side effect" :is any change to state or behavior that can be seen outside of returning a value from a function.  

Some common kinds of side effects are things like:  
- Logging a value to the console
- Saving a file
- Setting an async timer
- Making an AJAX HTTP request
- Modifying some state that exists outside of a function, or mutating arguments to a function
- Generating random numbers or unique random IDs (such as Math.random() or Date.now())  

Redux middleware were designed to enable writing logic that has side effects.  

### Redux Async Data Flow
Just like with a normal action, we first need to handle a user event in the application, such as a click on a button. Then, we call dispatch(), and pass in something, whether it be a plain action object, a function, or some other value that a middleware can look for.  
Once that dispatched value reaches a middleware, it can make an async call, and then dispatch a real action object when the async call completes.  
![Redux Async Data Flow](./Redux%20Async%20Data%20Flow.PNG)

## Redux Thunk
Thunk middleware for Redux. It allows writing functions with logic inside that can interact with a Redux store's dispatch and getState methods.  
A thunk is a function that wraps an expression to delay its evaluation.  

Redux Thunk middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. The inner function receives the store methods dispatch and getState as parameters.  

### Using Redux Thunk
The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.  

The key benefit provided by redux-thunk is it allows us to avoid directly causing side effects in our actions, action creators, or components.  
