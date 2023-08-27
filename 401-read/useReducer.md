# useReducer:
## What is the motivation for adding a reducer?
reducer in a software application, especially in the context of state management in frameworks like Redux, serves to centralize and manage changes to the application's state.
Reducers ensure a predictable and controlled way of updating state, enhancing code maintainability and facilitating debugging by isolating the logic responsible for state modifications.
This helps prevent data inconsistencies, improves collaboration among developers, and enhances the overall stability of the application.

## What are actions in the context of a reducer? How are they different than setting state directly?
In the context of a reducer, actions are objects that describe changes to an application's state. They provide a structured way to convey what specific update is required.
Unlike setting state directly, actions encapsulate intentions, making state changes traceable and enabling better debugging.
Reducers then interpret these actions and apply changes in a controlled manner, maintaining predictability and aiding in managing complex state logic.

## What common list operation is useReduce named for, and why?
useReducer in React is named for the common list operation "reduce," which is also known as "fold" in functional programming.
The operation involves iteratively applying a function to elements in a list, accumulating a result.
Similarly, useReducer in React iteratively applies a reducer function to the current state and an action, accumulating updates over time

## When should you switch from useState to useReducer?
1- State Logic Complexity: If your component's state transitions require logic that goes beyond simple updates, useReducer can help centralize and manage the complexity.

2- Multiple Actions: When you have multiple actions that affect the same state, useReducer allows you to handle them in a more organized and predictable manner.

3- Local vs. Global State: For global state management, or when multiple components need to interact with the same state, useReducer can provide better control and avoid prop drilling.
