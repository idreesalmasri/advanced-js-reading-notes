## React Hooks

what is a hook?
Hooks are the new feature introduced in the React 16.8 version. It allows you to use state and other React features without writing a class. Hooks are the functions which "hook into" React state and lifecycle features from function components. It does not work inside classes.

When to use a Hooks?
If you write a function component, and then you want to add some state to it, previously you do this by converting it to a class. But, now you can do it by using a Hook inside the existing function component.

Rules of Hooks
 you need to follow these two rules when using hooks These rules are:
 1. Only call Hooks at the top level
 2. Only call Hooks from React functions

## Hooks State
useState is a Hook . We call it inside a function component to add some local state to it. React will preserve this state between re-renders.
useState returns a pair: the current state value and a function that lets you update it. You can call this function from an event handler or somewhere else.

The only argument to useState is the initial state

The state here doesn’t have to be an object — although it can be if you want. The initial state argument is only used during the first render.

This example renders a counter. When you click the button, it increments the value:
``` 
import React, { useState } from 'react';

function Example() {
  // Declare a new state variable, which we'll call "count"
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```
Declaring multiple state variables
You can use the State Hook more than once in a single component:
```
function ExampleWithManyStates() {
  // Declare multiple state variables!
  const [age, setAge] = useState(42);
  const [fruit, setFruit] = useState('banana');
  const [todos, setTodos] = useState([{ text: 'Learn Hooks' }]);
  // ...
}
```

### Functional updates
If the new state is computed using the previous state, you can pass a function to setState. The function will receive the previous value, and return an updated value.
