# Application State with Redux

## What is the first principle of Redux?
### The first principle of Redux is "Single Source of Truth." This principle emphasizes that the entire state of your application should be stored in a single JavaScript object tree within a single store.
### This state tree is considered the "single source of truth" for your application's data.

## what is a store and what do we use our reducers for within that store?

### - "store" is a fundamental concept. It's an object that holds the entire state of your application. The store has several important responsibilities:

### - Holding State: The store contains the current state of your application as a single, immutable JavaScript object. This state represents the data and UI state of your application.

### - State Access: It provides a way to access the current state via a getState() method, allowing components and other parts of your application to read the data stored in the state.

### - State Updates: The store allows you to update the state by dispatching actions. Actions are plain JavaScript objects that describe what happened in your application. Reducers are used to specify how the state should change in response to these actions.

## Name three Redux store methods given to us by createStore and describe their use.

### - getState(): This method is used to retrieve the current state of the Redux store. It returns the entire state object
### - dispatch(action): The dispatch method is used to dispatch actions to the Redux store. Actions are plain JavaScript objects that describe what happened in your application.
### - subscribe(listener): The subscribe method allows you to register a listener function that will be called whenever the state in the Redux store is updated.

## Explain to a non-technical recruiter what combineReducers() does and why it is useful.
### is a utility function in Redux that simplifies state management. It takes multiple reducer functions, each responsible for a specific part of the application's state, and combines them into a single reducer. 
### This combined reducer handles the overall state of the application. This is useful because it helps organize and modularize the state management code, making it easier to maintain and scale as the application grows. 
### It also enforces a clear separation of concerns, improving code readability and collaboration among developers.

