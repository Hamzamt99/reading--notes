# React:
## What are the building blocks of a React app?
## *Components*: 

### There are two type of components :
#### 1- Functional Components
#### 2- Calss Components

### JSX:
#### It's a syntax extension for JavaScript that allows you to write HTML-like code within your JavaScript code
### Props and state: 
#### Props enable parent-child component interaction, while state is used by components to manage its behavior.

### Context :
#### is an advanced feature that provides a way to pass data through the component tree without having to manually pass props down at every level. 
#### It's primarily used when certain data needs to be accessible by many components at different levels of nesting.
#### React.createContext() function. This returns an object with two components: Provider and Consumer.

## What is the difference between an HTML element and a React component?
#### React components provide a higher level of abstraction, encapsulation of logic, and reusability compared to raw HTML elements.
#### They enable developers to build dynamic and interactive UIs more effectively by combining HTML-like structure with JavaScript logic.

## What is JSX and why do we use it?  
### JSX simplifies the process of building user interfaces in React by providing a more intuitive and expressive way to describe components' structure, content, and interactivity while seamlessly integrating JavaScript logic.

## Describe the process of embedding JavaScript expressions in JSX:

### JavaScript expressions within JSX allows you to dynamically generate content, compute values, and incorporate logic directly into your user interface components.
### This is achieved by wrapping the JavaScript expression in curly braces {} within your JSX code.

## Does React or JSX have any special features for iteration or conditional logic?

### Yes, both React and JSX have special features for iteration and conditional logic that allow you to handle lists of items and control the rendering of components based on conditions.

## How does React know to respond to a user’s inputs?
### React responds to a user's inputs by managing the state of components, re-rendering them when the state changes, and executing event handlers to update the UI in response to user interactions. 
### This approach helps create interactive and responsive user interfaces in React applications.

## What word indicates that a React component manages data with a Hook?
### useState is a built-in React Hook that allows functional components to manage and update state within the component.
### It is used to declare state variables and their initial values, as well as to provide functions for updating those state variables. 
### This Hook enables functional components to have state management capabilities similar to class components.

## How can two react components share data? 
### Two React components can share data in several ways, depending on the relationship between the components and the scope in which the data needs to be shared. Here are a few common methods:
1- Props
2- Context
3- State Lifting
4- Redux or State Management Libraries
5- Event Emitter Libraries
