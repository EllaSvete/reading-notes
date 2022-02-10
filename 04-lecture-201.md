# Class 04 Lecture Notes

## Function!

- a data type

### What is a function?

- A function is a group of statements that perform a task or calculate a value stored in a structure that prevents them from running until the function is 'called' or 'invoked'

### Why

- they're reusable
- prevent bugs
- make code dry (don't repeat yourself)

### 2 step process

- define/declare
- run/invoke

// function declaration

function greeting(){
  console.log('hey there class!');
}

greeting(); // calling the function, call after the function

// function expression - we won't be doing these!!

let newGreeting = function(){
  console.log('This is a new greeting!');
}

newGreeting();

- Functions

function nameGreeting(firstName, lastName){
  console.log(`Hey ${firstName} ${lastName}!`);

}

namedGreeting('Audrey', 'Patterson');

- function returns

function multiply(a,b){
  return a*b;
}

let product = multiply(2,2);

- order matters

function subtraction(a,b){
  return a-b;
}

let answer = subtraction(10,5); // if you switch numbers you would get -5

default parameters = 0 or = null

// function multiple returns

function sum(a,b){
  return [a+b, 'they were summed!']
}

let addition = sum(2+2);
console.log(addition);

#### CSS

- positioning


