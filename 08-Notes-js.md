
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

## Loops with Programs

What is a loop?

- a loop is a set of operations (one liner, or a bunch of lines of code, functions invocations )that you need to run ore than once
- purpose: do things more
- syntax: they look a lot like function signature, but instead of parameter, we have a couple of options.
- 3 types: for, while, do while

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

for (let times =50; times > 0; times = times -5) {
    console.log('this loop has run' + times + 'many times')}