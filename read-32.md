## context api

What is Context API?

> The React Context API is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux.

> In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

When to Use Context?
> Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

React context API: How it works?
> React.createContext() is all you need. It returns a consumer and a provider. Provider is a component that as it's names suggests provides the state to its children. It will hold the "store" and be the parent of all the components that might need that store. Consumer as it so happens is a component that consumes and uses the state.

How to use Context API?
- Create a folder under your app root named contexts (not required. just a convention)
- Create a file named <your context name>Context.js, e.g. userContext.js
= import and create a context like so:
```
import React, { createContext } from "react";
const UserContext = createContext();
```
- Create a component that will wrap the provider named Provider e.g. UserProvider
Example using React Hooks:
```
const UserProvider = ({ children }) => {
  const [name, setName] = useState("John Doe");
  const [age, setAge] = useState(1);
  const happyBirthday = () => setAge(age + 1);
  return (
    <UserContext.Provider value={{ name, age, happyBirthday }}>
      {children}
    </UserContext.Provider>
  );
};
```
- Create a higher order component to consume the context named: with e.g. withUser
Example using React Hooks:
```
const withUser = (Child) => (props) => (
  <UserContext.Consumer>
    {(context) => <Child {...props} {...context} />}
    {/* Another option is:  {context => <Child {...props} context={context}/>}*/}
  </UserContext.Consumer>
);
```
- Finally export them
```
 export { UserProvider, withUser };
 ```