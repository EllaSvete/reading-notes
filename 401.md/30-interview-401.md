# Interview questions

## 201

- Describe the difference between a function declaration and a function expression.
  - function declarations load before any code in executed
  - function expressions load only when the interpreter reaches that line of code

  - if you call a function expression before its loaded you'll egt an error, you have to call the function declaration instead

- Explain the concept of separation of concerns as pertains to web development, and the roles of HTML, CSS, and JavaScript.
  - each module or layer in an application should only be responsbile for one thing and should not contain code that deals with other things
  - reduced complexityt by breaking a large application down into smaller functionality.

- Define the term semantic HTML, give a few examples of semantic tags in HTML, and why we use them whenever possible.
  - HTML that introduces meaning to the web page rather than just presentation.
  - <p> is important to use because the browser knows how to display them. 

- Describe OOP (Object Oriented Programming) including how prototype chains work.
  - Object Orientated Programming is a paradigm that relies on the concept of classes and objects. It's used to structure a software program into simple reusable pieces of code blueprints wchi create instances of objects.

- How could you create new instances of an object?
  - use the new keyword
  - the keyword creates a new instances of an object that we assign variables and invoke methods

- What does the keyword ‘this’ belong to in OOP?
  - this refers to the current object in a method or constructor

- Talk about Built-In Objects including a. Browser Object Model, b. Document Object Model c. Global JavaScript Objects
  - browser object model: allows JS to talk to the browser
  - document object model: data representation of the objects that make up structure and content of a webpage
  - global object: an object that lives on the global scope of an appliation

- When a user interacts with the HTML on a web page, there are three steps involved in getting it to trigger the JavaScript code. Together these steps are event handling. Describe these three steps.
  - capturing phase (click)
  - target phase (call back function)
  - bubbling phase (change is shown)

- What does JavaScript’s JSON object do to JSON data and what does it convert a JavaScript object into?
  - Json is an object structures like JS objects

## 301

- Explain why we use templating in web development.
  - used to separate content from presentation in web deisgn for mass production web documents

- Describe the difference between imperative and declarative programming styles.
  - declarative prgramming is a paradigm that expresses the logic of computation without describing it's control flow. 
  - imperative programming is a paradigm that uses statements that change a programs state.

## 401

- What is “state”?
  - the state of an object is the combination of the original values in the object plus any modifications made to them

- Imagine I have no knowledge of web application development. Describe an example of client/server architecture for me.
          request         request
  - client <--> internet  <---> server
           response       response
  - client <---> middleware <---> database/server

- In as much detail as you can manage, describe what happens when I type a link into my address bar and hit “enter”
  - looks up location of the server that is hosting the site
  - makes a connection to that server
  - send a request to specific page
  - handles response from the server
  - renders the page and lets you interact

- A potential client comes to you with an idea for a web application, but no knowledge of how to implement it. Walk them through what you, as a developer, would recommend that they do to implement their idea into production. Include estimates of time and point out where they may expect to incur costs. Make sure you justify every decision; remember that your client has no technical knowledge, only an idea. You want to give them confidence that their idea can be implemented and work without imploding.

  - wireframe of that the client needs and wants
  - find apis and other potential costs
  - determine database
  - build out backend 
  - build out front end and styling
  - check in and adjust based on their budget and vision.

## Python

- Why does a Python dictionary have O(1) lookup time?
  - O(1) mean constant time regardless of size. a ditionarys keys must be unique and to look something up means you have te key. You'll only find the key you've specified

- What is a “generator” and when might it be useful? If you can, build one for me that demonstrates its usefulness.
  - Generator functions allow you to declare a function that haves like an iterator, allowing programmers to make an iterator in a simple way. 
  
