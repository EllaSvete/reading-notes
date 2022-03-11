
# Javascript

## review

functions:

- what are some examples of things that you would return?
  - any data that another function might need, or another operation requires
  - function sum(number1, number2) => number1 + number2
- why would you ever console log in a website?
  - give dvelopers a quick way to get feedback
- when do we create a new function?
  - every function should have one and only one responsibility, as soon as you're doing something that that function isn't responsible for it should be a new function, that way we can re-use function.
- strings are compares, and in most cases if the operands are not the same type, JavaScript attempts to convert them to an appropriate type of coparison.


- Assignment operators
  - assign value to it's left operand based on the value of its right operand. The simple assignment operator is (=) which assigns the value of its right operand to its left operand. example:
  x=f() is an assignment expression that assigns the value of f() to x.
- Assigning to properties
  - if the variable refers to an object, then the left-hand side of an assignment expression may make assignments to properties of that variable. example:
  let obj = {};

obj.x = 3;
console.log(obj.x); // Prints 3.
console.log(obj); // Prints { x: 3 }.

const key = "y";
obj[key] = 5;
console.log(obj[key]); // Prints 5.
console.log(obj); // Prints { x: 3, y: 5 }

-  + : increment one (plus)
- - : decrement one
- & : logical AND
- ||: logical OR
- ! : logical negation / inverse

- Comparison operators
  - compares its perands and returns a logical value based on whether the comparison is true. Operands can be numerical, string, logical, or object values.
 
  - < : less than
  - > : greater thn
  - '!=' : not equal to
  - !== : returns true is operands are of the same type but not equal, or are different type
  - '==': is equal to (only compares value)
  - '===': trictly equal to. (compare value and type)
  - <== : returns true if the left operand is less than or equal to the right operand
  - >== : returns true if the left operand is greater than or eual to the right operand



## Loops with Programs

What is a loop?

- a loop is a set of operations (one liner, or a bunch of lines of code, functions invocations )that you need to run ore than once
- purpose: do things more
- syntax: they look a lot like function signature, but instead of parameter, we have a couple of options.
- 3 types: for, while, do while
- offers a quick and easy way to do something repeatedly, they repeat an action some number of times.

* Different types of loops:
  
  - for statment- repeats loops until a specified condition evaluates to false
  - do while statement- repeats until specified condition evaluates to false
  - labeled statement- executes its statements as long as a specified condition evaluates to true.
  - break statement
  - continue statement
  - for...in statement
  - for... of statement 

'''js

//for loop

// 3 things that go here, the first in a variable
// the first is a variable which should e a number (initalizer)
// the second is a condition, when the condition is false the loop will stop
// the thirs is un update to the initalizer (incrementer)

// times-- == times - 1;

for (let times =5; times > 0; times--) {
    // this block will run as many times as the loop needs
    console.log('this loop has run' + times + 'many times');
} 
// this condition will run all the way to 1 because it is greater than 0


// While loop
//parentheses only contain a condition

let likesWatermelons = confirm('Do you like watermelons?");

for (let times == 10)

while (!likesWatermelons) {
   //console.log('i will never stop running') {
   likesWatermelons = confirm('Do you like watermelons?');
}

// likesWatermelons need to be "true" for the inverse to be false

let num = 0;

while(num != 10) {
 console.log(num);
   num++;
}

'''

let answer= prompt ('yes or no, do you like this?')

while (answer != 'yes' || answer != 'YES')


let num = 10;

do {
   console.log();
   num++;
} while (num < 10)

for (let i =50; i > 0; i = i -5) {
    console.log('this loop has run' + times + 'many times')}