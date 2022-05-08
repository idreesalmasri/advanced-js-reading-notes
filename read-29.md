## Advanced State with Reducers

useReducer: is one of the additional Hooks that shipped with React v16.8. An alternative to the useState Hook, useReducer helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux, Recoil or MobX. In certain cases, it is an outright better option.

How does the useReducer Hook work?
The useReducer Hook is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.useReducer returns an array that holds the current state value and a dispatch function to which you can pass an action and later invoke it.


 initialize state with the useReducer Hook:
 ``` 
 const initialState = { count: 0 }

const [state, dispatch] = useReducer(reducer, initialState) 
```

The reducer function:
The reducer function itself accepts two parameters and returns one value. The first parameter is the current state, and the second is the action. The state is the data we are manipulating. The reducer function receives an action, which is executed by a dispatch function:
```
function reducer(state, action) { }

dispatch({ type: 'increment' })
```
The action is like an instruction you pass to the reducer function. Based on the specified action, the reducer function executes the necessary state update.


The dispatch method
> The dispatch function accepts an object that represents the type of action we want to execute when it is called. Basically, it sends the type of action to the reducer function to perform its job, which, of course, is updating the state.


useState vs. useReducer

> useState is a basic Hook for managing simple state transformation, and useReducer is an additional Hook for managing more complex state logic. However, it’s worth noting that useState uses useReducer internally, implying that you could use useReducer for everything you can do with useState.  
However, there are some major differences between these two Hooks. With useReducer, you can avoid passing down callbacks through different levels of your component. Instead, useReducer allows you to pass a provided dispatch function, which in turn will improve performance for components that trigger deep updates.

When to use the useReducer Hook?
> As your application grows in size, you’ll most likely deal with more complex state transitions, at which point you’ll be better off using useReducer.  
useReducer provides more predictable state transitions than useState, which becomes more important when state changes become so complex that you want to have one place to manage state, like the render function.