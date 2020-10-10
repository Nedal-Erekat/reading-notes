# Component Based UI

## Review, Research, and Discussion

* Name 5 Javascript UI Frameworks (other than React)
 1. Angular
 2. Vue
 3. Ember
 4. Ext JS by Sencha

* What’s the difference between a framework and a library?
 - Frameworks and libraries are both code written by someone else that helps you perform some common tasks in a less verbose way.
 - A framework inverts the control of the program. It tells the developer what they need. A library doesn’t. The programmer calls the library where and when they need it.

- `Rendering` is the process of gathering data (if any) and load the associated templates (or just send the output directly). Then apply the gathered data to the associated templates. The final output is sent to the user.

- `template` is a generic class or other unit of source code that can be used as the basis for unique units of code.

- `state` of a program at a given time refers to a snapshot of all the data the program is currently looking at or analyzing to get to the next step in it's execution.


- `JSX` it is a syntax extension to JavaScript,tag syntax is neither a string nor HTML.
- Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both
- You can put any valid JavaScript expression inside the curly braces in JSX
- React DOM uses camelCase property naming convention instead of HTML attribute names.
- JSX Prevents Injection Attacks, React DOM escapes any values embedded in JSX before rendering them.

### React Only Updates What’s Necessary
React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.

### Rendering an Element into the DOM
To render a React element into a root DOM node, pass both to `ReactDOM.render():`,  Once you create an element, you can’t change its children or attributes. 

```
const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));
```

### Components and Props
Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.

> Note: Always start component names with a capital letter. React treats components starting with lowercase letters as DOM tags. For example, `<div />` represents an HTML div tag, but `<Welcome />` represents a component and requires Welcome to be in scope.

