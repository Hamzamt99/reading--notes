# Asynchronous Actions:
## Why use Redux middleware? 

Redux middleware is a crucial part of the Redux library that provides a way to extend the behavior of the Redux store and the actions that flow through it.
Middleware sits between the dispatching of an action and the moment it reaches the reducer,
allowing you to intercept, modify, or otherwise handle actions in a controlled and reusable manner. 

## Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.

The Redux Async Data Flow Diagram describes how data flows through a Redux-based application when dealing with asynchronous operations,
such as fetching data from an API. 

## How are we accommodating async in our Redux app?

Accommodating asynchronous operations in a Redux app involves using middleware and certain patterns to manage data flow and
state updates when dealing with actions that are not purely synchronous.

## Why would you need redux-thunk middleware?
1- Handling Asynchronous Operations
2- Encapsulation of Async Logic
3- Cleaner Code

## Redux Thunk middleware allows you to write action creators that return a function instead of an action.

## Describe how any return value from the inner thunk function will be made available.

In Redux, the return value from the inner thunk function is made available through a mechanism called "dispatch." 
The dispatch function is provided by the Redux store and is used to send actions to the store, which in turn triggers the reducer to update the state.
