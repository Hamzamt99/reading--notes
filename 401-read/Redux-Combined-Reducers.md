# Redux-Combined-Reducers.md

## Why create multiple reducers?

To improve code organization, maintainability, and scalability.

## How would you combine multiple reducers?

Redux provides a utility function called `combineReducers` to combine multiple reducers into a single root reducer.

## How will you manage state as an immutable object? why?

Managing state as an immutable object is a common practice in many state management libraries and paradigms, including Redux, React's `useState`, and functional programming in general.

## `combineReducers` is a utility function to simplify the most common use case when writing Redux reducers.

## Explain how `combineReducers` assembles the new state tree

`combineReducers` in Redux is a utility function that combines multiple reducers into a single reducer function. 
It's commonly used to manage different parts of the application state in a more modular way.

## How would you define initial state in an app using combineReducers?

```javascript
// counterReducer.js
const initialState = {
  count: 0,
};

// userReducer.js
const initialState = {
  user: null,
};

// productReducer.js
const initialState = {
  products: [],
};.

Why will you want to split your reducing functions as your app becomes more complex?
Splitting your reducing functions, often referred to as reducers,
as your app becomes more complex is a recommended practice in Redux and other state management systems for several important reasons:

Modularity and Organization
Maintainability
Reusability
The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.
What is a popular convention when naming reducers?
A popular convention when naming reducers in Redux is to use descriptive and consistent naming patterns to make your code more readable and maintainable.
