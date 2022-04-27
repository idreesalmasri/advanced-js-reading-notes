## Effect Hook

* The useEffect Hook allows you to perform side effects in your components.
* Some examples of side effects are: fetching data, directly updating the DOM, and timers.
* useEffect accepts two arguments. The second argument is optional.
* useEffect(<function>, <dependency>)

Data fetching, setting up a subscription, and manually changing the DOM in React components are all examples of side effects. Whether or not you’re used to calling these operations “side effects” (or just “effects”).
Common side effects include:

* Making a request to an API for data from a backend server
* To interact with browser APIs (that is, to use document or window directly)
* Using unpredictable timing functions like setTimeout or setInterval


There are two common kinds of side effects in React components: those that don’t require cleanup, and those that do.

* Effects Without Cleanup
* Effects with Cleanup

What does useEffect do? 
By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed , and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API.

Why is useEffect called inside a component?
Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect. We don’t need a special API to read it — it’s already in the function scope. Hooks embrace JavaScript closures and avoid introducing React-specific APIs where JavaScript already provides a solution.

Does useEffect run after every render?
By default, it runs both after the first render and after every update. (We will later talk about how to customize this.) Instead of thinking in terms of “mounting” and “updating”, you might find it easier to think that effects happen “after render”. React guarantees the DOM has been updated by the time it runs the effects.

The correct way to perform the side effect in our User component is as follows:

* We import useEffect from "react"
* We call it above the returned JSX in our component
* We pass it two arguments: a function and an array
