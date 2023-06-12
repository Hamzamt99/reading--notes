# Express REST API 
## ES6 Classes 

### Classes are a template for creating objects.

### Can a class declaration be hoisted?

#### In JavaScript, unlike function declarations, class declarations are not hoisted to the top of their containing scope. This means that you cannot access or use a class before it is declared in your code.

### How would you describe a constructor and contextual “this” to a non-technical friend?

#### Imagine you're building a house. You have a blueprint that describes how the house should look, with all the rooms, windows, and doors. The blueprint is like a class in programming. It defines the structure and behavior of the house, but it doesn't actually create a physical house.
#### Now, a constructor is like a special worker who takes the blueprint and builds an actual house based on it. The constructor knows how to follow the blueprint and create a real house with all the details specified in it.

#### The contextual "this" refers to the current object that is being created or manipulated. It allows the constructor or any method within the class to access and modify the properties and behaviors of that specific object.

## Using Express Routing

### Within Express, what does routing refer to?

#### In the context of Express, routing refers to the process of mapping incoming HTTP requests to specific handlers or functions that will handle those requests. It involves defining routes that specify the combination of URL paths and HTTP methods that the server should respond to.

### What is the difference between a route path and a route method?
#### A route path in Express refers to the URL pattern or pattern-matching string used to define the URL structure for a specific route.
### A route method in Express refers to the HTTP method (GET, POST, PUT, DELETE, etc.) used to handle a specific route.
### In summary, the route path defines the URL structure, while the route method defines the HTTP method used to handle that specific URL path.

### When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter? 

#### In Express, the next parameter is used to pass control to the next middleware function or route handler in the chain. It is appropriate to add next as a parameter to a route handler or middleware when you want to delegate control to the next function in the middleware stack.

## Express Routing 

### What is an Express Router?

#### An Express Router is a middleware in Express that allows you to define and organize routes separately, providing a modular approach for handling different URL paths and HTTP methods in your application.

### 

#### To initialize an Express Router in an Express server, you typically follow these steps:

##### 1- Import the Express module and create an instance of the Express Router

##### 2- Define routes on the router instance using the HTTP methods (get, post, etc.) and path patterns

##### 3- Mount the router on the Express application to make the routes available

### 4- What do we use route middleware for?

#### Route middleware in Express is used for:

##### 1- Authentication and authorization checks.
##### 2- Request validation and data parsing.
##### 3- Logging, error handling, and other common functionalities applied to specific routes or groups of routes.

## Reflection

## What are your learning goals after reading and reviewing the class README?

### Know more about express router and how can we use in Authentication and authorization