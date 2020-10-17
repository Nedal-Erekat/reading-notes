# Hooks API

![React](https://hackernoon.com/hn-images/1*HSisLuifMO6KbLfPOKtLow.jpeg)

Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.
Hooks are functions that let you “hook into” React state and lifecycle features from function components. 
> Hooks don’t work inside classes - they let you use React without classes.

When would I use a Hook? If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component. We’re going to do that right now!

- Components are more powerful, but they have to render some UI. This makes them inconvenient for sharing non-visual logic. 
-  Hooks let you use React features (like state) from a function — by doing a single function call. 
- Since Hooks are regular JavaScript functions, you can combine built-in Hooks provided by React into your own “custom Hooks”.  This lets you turn complex problems into one-liners and share them across your application
- Hooks don’t work inside classes. But you can use them instead of writing classes.


## UseState hook
 useState returns a pair: the current state value and a function that lets you update it. You can call this function from an event handler or somewhere else. It’s similar to this.setState in a class,except it doesn’t merge the old and new state together.
 The only argument to useState is the initial state. 
 > Normally, variables “disappear” when the function exits but state variables are preserved by React.

- If we wanted to store two different values in state, we would call useState() twice


## Effect Hook
You’ve likely performed data fetching, subscriptions, or manually changing the DOM from React components before. We call these operations “side effects” (or “effects” for short) because they can affect other components and can’t be done during rendering.
 * By default, React runs the effects after every render

## Rules of Hooks

call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions. call Hooks from React function components. Don’t call Hooks from regular JavaScript functions. 

## useEffect
useEffect lets us express different kinds of side effects after a component renders. Some effects might require cleanup so they return a function
Other effects might not have a cleanup phase, and don’t return anything.

There is no special code for handling updates because useEffect handles them by default. It cleans up the previous effects before applying the next effects. 

```
useEffect(() => {
  document.title = `You clicked ${count} times`;
}, [count]); // Only re-run the effect if count changes
```
### Optimizing Performance by Skipping Effects
In the example above, we pass [count] as the second argument. What does this mean? If the count is 5, and then our component re-renders with count still equal to 5, React will compare [5] from the previous render and [5] from the next render. Because all items in the array are the same (5 === 5), React would skip the effect. That’s our optimization.