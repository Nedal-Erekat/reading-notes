
## Actions

By default, Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects. Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers

Usually, for any API request you'll want to dispatch at least three different kinds of actions:
1. An action informing the reducers that the request began.
2. An action informing the reducers that the request finished successfully.
3. An action informing the reducers that the request failed.

## Async Action Creators
Finally, how do we use the synchronous action creators we defined earlier together with network requests? The standard way to do it with Redux is to use the Redux Thunk middleware. It comes in a separate package called redux-thunk. 

- by using this specific middleware, an action creator can return a function instead of an action object.This way, the action creator becomes a thunk.

# Thunk
Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation.
```
import { createStore, applyMiddleware } from 'redux';
import thunk from 'redux-thunk';
// use applyMiddleware to add the thunk middleware to the store
const store = createStore(rootReducer, applyMiddleware(thunk));
```
## Using Redux Thunk in a Sample Application
The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.