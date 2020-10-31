# Redux Toolkit in Action

How to convert "plain Redux" code to use RTK
How to use RTK in a typical React+Redux app
How some of the more powerful features of RTK can be used to simplify your Redux code

```
# If you're using NPM:
npm install @reduxjs/toolkit
import { createSlice } from '@reduxjs/toolkit'

```
## Converting the Store to Use configureStore(rewriting the app)
Just like with the "counter" example, we can replace the plain Redux createStore function with RTK's configureStore. This will automatically set up the Redux DevTools Extension for us.

## Understanding Slices
 A normal Redux application has a JS object at the top of its state tree, and that object is the result of calling the Redux combineReducers function to join multiple reducer functions into one larger "root reducer"

## Writing the Slice Reducer
createSlice takes an options object as its argument, with these options:
name: a string that is used as the prefix for generated action types
initialState: the initial state value for the reducer
reducers: an object, where the keys will become action type strings, and the functions are reducers that will be run when that action type is dispatched. (These are sometimes referred to as "case reducers", because they're similar to a case in a switch statement)

Notice that the addTodo reducer is calling state.push(). Normally, this is bad, because the array.push() function mutates the existing array, and Redux reducers must never mutate state!.
 knows this object was updated, and makes copies of both the todo object and the containing array.

> createSlice returns an object that looks like this:

```
{
  name: "todos",
  reducer: (state, action) => newState,
  actions: {
    addTodo: (payload) => ({type: "todos/addTodo", payload}),
    toggleTodo: (payload) => ({type: "todos/toggleTodo", payload})
  },
  caseReducers: {
    addTodo: (state, action) => newState,
    toggleTodo: (state, action) => newState,
  }
```
* Notice that it auto-generated the appropriate action creator functions and action types for each of our reducers - we don't have to write those by hand!