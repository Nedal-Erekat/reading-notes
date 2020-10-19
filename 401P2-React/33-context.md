# Context
Context provides a way to pass data through the component tree without having to pass props down manually at every level. Context is primarily used when some data needs to be accessible by many components at different nesting levels.

## When to Use Context
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

- Use a Provider to pass the current theme to the tree below.Any component can read it, no matter how deep it is.

- `component composition`to avoid passing some props through many levels.

> const MyContext = React.createContext(defaultValue);
> `<MyContext.Provider value={/* some value */}>`

## Updating Context from a Nested Component
It is often necessary to update the context from a component that is nested somewhere deeply in the component tree. In this case you can pass a function down through the context to allow consumers to update the context
