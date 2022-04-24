## Reading: Component Based UI

### Introducing JSX
- JSX:it is a syntax extension to JavaScript.We recommend using it with React to describe what the UI should look like.jsx comes with the full power of JavaScript.

- JSX produces React “elements”.
### Why JSX?
- React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.
- Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. 

- JSX allows React to show more useful error and warning messages.

What is JSX?
- JSX stands for JavaScript XML.
- JSX allows us to write HTML in React.
- JSX makes it easier to write and add HTML in React.

- JSX allows us to write HTML elements in JavaScript and place them in the DOM without any createElement()  and/or appendChild() methods.
- JSX converts HTML tags into react elements.
- JSX is an extension of the JavaScript language based on ES6, and is translated into regular JavaScript at runtime.

### Rendering Elements
Elements are the smallest building blocks of React apps.element describes what you want to see on the screen.

- Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

#### Updating the Rendered Element
React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.
With our knowledge so far, the only way to update the UI is to create a new element, and pass it to root.render().



