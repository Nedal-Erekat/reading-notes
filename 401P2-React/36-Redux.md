# Redux
State management is absolutely critical in providing users with a well-crafted experience with minimal bugs.

Redux provides a solid, stable and mature solution to managing state in your React application. Through a handful of small, useful patterns, Redux can transform your application from a total mess of confusing and scattered state, into a delightfully organized, easy to understand modern JavaScript powerhouse.


- any data get to redux app done by actions like events
- the function in redux should be pure(preductaple), like the it does not affect on the arrgument or has side effects like calling the database or changing the arguments of the functions
> we have to write a function thet take the previous state and the action have been dispatch and return the next state of the app and the function has to be pure; this function is called the `reducer`.

- create store function provieded by redux has 3 methods:
 - getstate() 
 - dispatch() ---> to make an action
 - subscribe() ---> to rerunder our app with currne  state

> the most important thing during our working on redux is to make sure that our code is free of notaion(it has not any effect on the original values like arrays using push or splice )
 - insted using `push()` we can use `concat()`.
 - sepred operator would be usefull with arrays and `Object.assign()` with objects

