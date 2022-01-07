
# Programming

## How do you put on a jacket

define a function for putting on a  jacket:

- What Jacket? What is a jacket?

- make sure unzipped
- make sure right side up
- etc.

## Definte Functions

Any js operation/ set of operations that should be repeated. Provides a syntax for turning operations into a repeatable "thing"

- JS function signature - what are the characters that g o into a function
- Anonymous function doesn't have a name

Below will help us not repeat the same thing over and over again:

'''js
// "function" keyword, followed by a name for the function, followed by parentheses followed by a pair of curly brakets.

// this is defing a variable
let wordsVariable = 'is it morning yet';

function calculateTime(time){
    // the things the function needs to do go here.

if (time < 12){ // an expression
    return 'it is morning';
} else{
    return 'it is the evening';
  }
}
return 'thanks for those words'; // this return gives a value to anything outside of the curlies

}
// invoke functionName
functionName('Is it morning yet'); // our argument


'''

- parameters/arguments
  - Arguments are the values that are passed into the function on 'invocation'.
  confirm ('is it the morning?")
  - Arguments are Value asigned to parameter
  - Arguments can be anything if it can be defined in JavaScript
  - Parameter is the variable defined in the parentheses in our function signature
- return value
  - stops your function from running

## Aditional js scripting topics

- expressions : a line of code or js operations that evaluates to some value. Only that parts that evaluates like words > 10
'''js

   let words = 'name';
   of (words > 10) {
    console.log('works');
   } else{
    console.log('doesn't work');
   }
    let is Awesome = false;

    if (!isAwesome) {
        console.log ('You are awesome');
    }

'''

- operators: 
  - < : less than
  - > : greater thn
  - + : increment one (plus)
  - - : decrement one
  - & : logical AND
  - ||: logical OR
  - ! : logical negation / inverse
    - '!=' : not equal to
- '==': is equal to (only compares value)
- '===': trictly equal to. (compare value and type)

'''js

let number = 10;

if (number < 10 && number > 5) {
    console.log('your number is between 5 and 10');
} else {
    console.log('your number is not between 5 and 10');
}

function compareNumber(number){
if (number < 10 && number > 5) {
    console.log('your number is between 5 and 10');
} else {
    console.log('your number is not between 5 and 10');
}
  return 1;
}

function makeASandwich(){

    let bread = prompt('what bread would likke?');
    let meat = prompt('what meat would you like?');
    let cheese = prompt('what cheese do you like?');

    return 'Here is a sandwich with' + bread + ',' + meat + ',' + cheese + '.';
}
'''