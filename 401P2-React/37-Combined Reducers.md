# combineReducers(reducers)
As your app grows more complex, you'll want to split your reducing function into separate functions, each managing independent parts of the state.

The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers()

## Arguments#
reducers (Object): An object whose values correspond to different reducing functions that need to be combined into one. See the notes below for some rules every passed reducer must follow.

## Returns#
(Function): A reducer that invokes every reducer inside the reducers object, and constructs a state object with the same shape.