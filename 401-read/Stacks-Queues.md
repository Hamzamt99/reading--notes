# WHY the stack and the queues:

## tacks and queues are data structures that allow efficient manipulation of collections of elements. They have different characteristics and are used in various scenarios depending on the requirements of the problem at hand.

## A stack is an ordered collection of elements where the addition and removal of elements follow the "last-in, first-out" (LIFO) principle. This means that the last element added to the stack is the first one to be removed. 
## Think of it like a stack of books where you can only add or remove books from the top.
## JavaScript arrays can be easily used as stacks by using the push() method to add elements to the end of the array and the pop() method to remove the last element.

# WHAT is the Stacks and Queues?

## 1- Stack:

### A stack is an ordered collection of elements where the addition and removal of elements follow the "last-in, first-out" (LIFO) principle.
### Imagine a stack of books where you can only add or remove books from the top.
### The last element added to the stack is the first one to be removed.
### Elements can be added to the top of the stack (often called "pushing" onto the stack) and removed from the top (often called "popping" from the stack).
### Examples of real-life stacks include the call stack in programming and the browser history.

## 2-Queue:

### A queue is an ordered collection of elements where the addition of elements is done at one end called the "rear" (also known as "enqueue"), and the removal of elements is done from the other end called the "front" (also known as "dequeue").
### The elements in a queue follow the "first-in, first-out" (FIFO) principle, similar to a line of people waiting for their turn.
### The first element added to the queue is the first one to be removed.
### Elements are added to the rear of the queue and removed from the front of the queue.
### Examples of real-life queues include waiting in line at a ticket counter or a queue of tasks to be processed.

# HOW:

*Implementing a Stack or Queue using Arrays:
JavaScript arrays can be used to implement both stacks and queues. Here's how you can use arrays to create a stack or a queue:*

### Stack:

javascript
Copy code
// Create an empty stack using an array
const stack = [];

// Adding elements to the stack using the push() method
stack.push(1);
stack.push(2);
stack.push(3);

// Removing elements from the stack using the pop() method
console.log(stack.pop());  // Output: 3
console.log(stack.pop());  // Output: 2
console.log(stack.pop());  // Output: 1
### Queue:

javascript
Copy code
// Create an empty queue using an array
const queue = [];

// Adding elements to the queue using the push() method
queue.push(1);
queue.push(2);
queue.push(3);

// Removing elements from the queue using the shift() method
console.log(queue.shift());  // Output: 1
console.log(queue.shift());  // Output: 2
console.log(queue.shift());  // Output: 3
In the array implementation, the push() method is used to add elements to the stack or queue, and the pop() method is used to remove elements from the stack. For queues, you can use the shift() method to remove elements from the front of the array.
