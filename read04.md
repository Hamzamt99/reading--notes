# What is the javascript?
*JavaScript is a web-based scripting language. It is an interpreted language, which means that unlike C or C++, it does not require a compiler to translate its code. JavaScript is a scripting language that runs in a web browser.
ECMAScript 2018 is the most recent version of the language, which was published in June 2018.
To create web apps or web pages, JavaScript is used in conjunction with HTML and CSS. Most current web browsers, such as Google Chrome, Firefox, Safari, Microsoft Edge, Opera, and others, support JavaScript. JavaScript is currently supported by the majority of Android and iPhone browsers.
JavaScript controls the dynamic elements of web pages. It works in web browsers and, more recently, on web servers as well. Application Programming Interfaces (API) are also supported by JavaScript, giving you more functionality.
Understanding all the ways JavaScript works is a little easier when you understand how web programming works, so let's learn more.*
## How Does JavaScript Work?
Before writing JavaScript it's important to know how it works under the hood. There are two important pieces to learn about: How the web browser works, and the Document Object Model (DOM).

![Js](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2017/09/how-works.png?q=50&fit=crop&w=750&dpr=1.5)

*A web browser loads a page, parses the HTML, and generates a Document Object Model (DOM) from the contents. The DOM gives your JavaScript code a live view of the web page.
The browser will then acquire any pictures or CSS files that are connected to the HTML. The CSS parser provides the CSS information.
The DOM assembles the HTML and CSS to build the web page initially. The JavaScript engine in the browser then loads JavaScript files and inline code, but does not run it right away. It waits for the HTML and CSS to load completely.*


## What Can I Do With JavaScript?
JavaScript is a full-fledged programming language that can do most things a regular language like Python can do. These include:
+ Declaring variables.
+ Storing and retrieving values.
+ Defining and invoking functions, including arrow +  functions.
+ Defining JavaScript objects and classes.
+ Loading and using external modules.
+ Writing event handlers that respond to click events.
+ Writing server code.
And much more.

## Let's look at some JavaScript basics with code examples:

+ Declaring variables

let num = 5;
let myString = "Hello";
var interestRate = 0.25;

+ Operators
Addition

12 + 5
>> 17

+ Arrays
let myArray = [1,2,4,5];
let stringArray = ["hello","world"];

+ Functions
JavaScript can write functions, here's a simple function that adds numbers.

function addNumbers(num1,num2){
return num1 + num2;
}
>> addNumbers(10,5);
>> 15

+ Loops
JavaScript can perform loops for iteration, loops like for loops and while loops.

for(let i = 0; i < 3; i++){ 
console.log("echo!"); 
} 
>> echo!
>> echo!
>> echo!
let i = 0;
while(i < 3) { 
console.log("echo!");
i++; 
} 
>> echo!
>> echo!
>> echo!

+ Comments
// Writing a comment
/*Writing a multi-line comment
You can use as many lines as you like
to break up text and make comments more readable
*/


