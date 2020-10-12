# Component Composition

1. The Component Lifecycle
By far the most important concept on this list is understanding the component lifecycle. The component lifecycle is exactly what it sounds like: it details the life of a component. Like us, components are born, do some things during their time here on earth, and then they die 

2. Higher-Order Components
A higher-order component is a function that takes a component and returns a new component.

3. React State and setState()
Most of you have probably used React state, we even used it in our HOC example. But it’s important to understand that when there’s a state change, React will trigger a re-render on that component (unless you specify in shouldComponentUpdate to say otherwise).

4. React Context
This brings us now to React context which is just global state for components.

The React context API allows you to create global context objects that can be given to any component you make. This allows you to share data without having to pass props down all the way through the DOM tree.