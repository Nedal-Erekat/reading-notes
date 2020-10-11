# React_Props and State


### Review, Research, and Discussion
1. Does a deployed React application require a server?

React. js does not use a web server to create virtual DOMs. It builds the virtual DOM and does its diff operations on the client's browser.

## Components and Props
Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.
Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

## Handling Events
Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

React events are named using camelCase, rather than lowercase.
With JSX you pass a function as the event handler, rather than a string.

## Forms
HTML form elements work a little bit differently from other DOM elements in React, because form elements naturally keep some internal state.

## React Testing Library
React Testing Library (RTL) is made of simple and complete React DOM testing utilities that encourage good testing practices