# Redux - Additional Topics
## What concerns are addressed by Redux Toolkit?
Redux Toolkit addresses concerns related to boilerplate code, store setup, and efficient state management in Redux applications.
It simplifies the configuration of Redux stores, reduces redundant code, and promotes best practices like immutable state updates, making it easier to maintain and scale Redux-based applications.

## What does configureStore() do?
is a function provided by Redux Toolkit that simplifies the setup of a Redux store in a Redux application.
It combines several Redux store configuration steps into a single function call, such as creating the store

# MobX

## What is Mobx?
Mobx is a state management library for JavaScript and React applications. It provides a simple and efficient way to manage the state of your application by using observable objects,
computed values, and reactions.
Mobx is often used as an alternative to Redux for state management in React applications.

## How does MobX make it “impossible” to produce an inconsistent state?
Mobx helps make it "impossible" to produce an inconsistent state through its reactive and observable model.

## How would we build a reactive user interface?
Setup:

Begin by setting up your project with the necessary tools. Create a new React application using create-react-app or any other method you prefer.
State Management with Mobx:

Integrate Mobx into your React application. You can install Mobx and Mobx React bindings via npm or yarn:

bash
Copy code
npm install mobx mobx-react
Define your application's state using Mobx observables. These observables represent the data your UI will react to.

Create Mobx actions to modify the state. Actions should be the only way to change the state in a Mobx-driven application. You can use decorators like @observable, @action, and @computed to define your state and actions.

Reactive Components:

Design your UI components to be reactive. Use Mobx React's observer higher-order component (HOC) to wrap your components, making them automatically react to changes in observables.

Inside your components, access and render data from Mobx observables. Any changes to the observables will trigger component re-renders automatically.

Reactions and Computed Values:

Define computed values in Mobx to derive data from your observables. These computed values will stay up-to-date as their dependencies change.

Create Mobx reactions using autorun or other reaction types to run specific code when certain observables change. This allows you to respond to state changes with custom logic.

Actions:

Implement actions for user interactions, such as form submissions, button clicks, or other events. Actions should modify the Mobx state and trigger updates in the reactive components.

## How would I use createSlice()?
```javascript
import { createSlice } from '@reduxjs/toolkit';

// Create a Redux slice named 'myReducerName'
const mySlice = createSlice({
  name: 'myReducerName',
  initialState: {/* Initial state here */},
  reducers: {
    // Define your reducer functions here
    myAction: (state, action) => {
      // Update the state based on the action payload
    },
  },
});

// Export the 'myAction' action creator
export const { myAction } = mySlice.actions;

// Export the reducer function
export default mySlice.reducer;

