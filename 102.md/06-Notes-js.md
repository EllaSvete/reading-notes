
## JS

* JavaScript is prototype-based & single threaded

* What is a programming language?
  * telling a computer what to do using features that computers have available to them.

* Where does javascript run?
  * in web browsers

* The awuthor must include JS code in the html page that the user recieves. The JS code would run in the browser(aka the clinet side) 

* There are 3 major parts of what Javascript refers to 
   * The language itself
   * The DOM API- how the language can interactwith various parts of a web page in the browser. 
   * The server API 

* Any text edutor can be used
* You can either embed JS code directly inside of HTML file, or you can put a line in the HTML file that will include the external JS link.
* alert function is the most simple way to interact with JS code running in the browser - rarely used but shows the function of Javascript
* docuent.write function to change the content of the page - used to change what is shown
* 

- HTML is content
- css is look
- Javascript is behavior
  
  - Syntax is more apporachable. Characters are more traight forward for a programming language. 
  - Creating boxes, adding data, talking to another computer such as Netflix.

### Fundamental concepts

- Data types
  - string: group of text characters (numbers included) used to represent natural language, like a sentence always in single or double quotations
  - number: a quantitative value that represents all integers and decimals, and fractions
    - 1 or 1/2 or 4.5 or -1, 40000(no coma)
  - boolean: true and false
    - truthiness and falsiness javascript can evaluate certain things without being set as true or false
  - null and undefined

- Browser Behaviors - pre-built
  - Print text to the console
  - prompt user with a input box
  - Making http requests.
    - http is protocol that passes requests
- make decisions based on conditions
- You can work right into console
- the word "let" allows the word and lets you change variables. = gives it data and then it becomes a string
- let is Javascripts keyword and is a good default
- type always better
- Javascript is loosely tyed which means we can change what type a variable has
- semicolons are option, but should be consistent - JS lets you choose
- when to use the curly brackets: when you want to log a conditional functions. when i want something to happen only when something else happens. The thing the function does is within {}

### First Class Functions

- First-class functions are functions in language that are treated like any other variable.
- Variable is reference to a value
- Use the variable to invoke the function by adding parenthese at the end.
- Passing the function as an arugment to another function explains how we are treating the function as a value.
- Using double parentheses to invoke the returned function as well.
- confirm inctructs the browser to display a dialog with an optional message
- prompt method is used to display an optional message prompting the use to input text
- If you declare

#### Data types

- number!
  - let myValue = 6
- strings - sequence of characters
  - myName = "banana" <-- quotes make it known to be a string
- boolean - true / false
  - let myBoolean = false


#### Conditionals

- Conditional logic is 
if else

## Variable Examples

'let name  = 'Jacob';

if (age >= 31) {
    document.write('You're old!')
} else { (age <= 31)
    document.write('Too young!')
}

let content = document.getElementById('content-1');
console.log(content); // this is how you check it is sent to JS console
content.innerText = age;

< h1 id='title'>< /h1>

< script >
       let email = prompt( 'what is you your favorite email?');
       console.log('Sending email to: , email');
       document.write(email);
        < /script >
        
      // delcare variable to store what is grabbed by our function 
        document.getElementById('')// looks through code and looks for first thing it find that has ID and grabs that between parentheses.

