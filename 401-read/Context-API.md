# Context API
## Summarize the five principles for structuring state:
### - Group related state:
   If you always update two or more state variables at the same time, consider merging them into a single state variable.
### - Avoid contradictions:
in state. When the state is structured in a way that several pieces of state may contradict and “disagree” with each other, you leave room for mistakes. Try to avoid this.
### - Avoid redundant state: 
If you can calculate some information from the component’s props or its existing state variables during rendering, you should not put that information into that component’s state.
### - Avoid duplication in state: 
When the same data is duplicated between multiple state variables, or within nested objects, it is difficult to keep them in sync. Reduce duplication when you can.
### - Avoid deeply nested state:
Deeply hierarchical state is not very convenient to update. When possible, prefer to structure state in a flat way.

## What problem do Contexts aim to solve?
#### Contexts aim to solve the problem of maintaining relevant and coherent conversations in AI chat systems by allowing users to specify a conversation's context and history explicitly,
#### ensuring more accurate responses and meaningful interactions.

## What is one technique to try before useContext?
#### One technique to try before using useContext in React is to use prop drilling, where you pass data down through component props.
#### This can work well for smaller applications or when context is not needed globally throughout the application.

## What hook complements useContext for complex applications?
#### useReducer complements useContext for complex applications.
#### It allows you to manage more complex state logic in a predictable and centralized manner when combined with a context to share the state across components.
