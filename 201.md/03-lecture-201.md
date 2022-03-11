# Class 3

## Code review

### Counters

- let counter = 0; <-- global variable
  - every time we get a correct answer you do counter = counter + 1;
  new val = 0 + 1 which means counter then equals one
  old value of counter is 1 so then the new val would be 2

- you can also do counter++ which will increment it by 1

## Lecture

### Arrays

- Data type// data structure (typeof array) -> object **special type of object**
- a collection, a list of elements - can be mixed
  - strings, numbers, booleans, arrays, objects
- in JS we don't have to redetermine the size of the array
- Every element in the array has an index(location reference) that we can use to find where it is in the array
  - JS arrays are a zero based index system

- Built in methods
  - Methods are `.name()`
  - `.push()`, `.pop()`
- Property
  - `,length`

let myArr = [1, 'hello', [1,2,5]];

console.table(myArr); // this will give you your indexes


//.               0        1             2          3
let students = ['Cole', 'Dwight', 'Christopher', 'Abdi']

let dwight = students[1]
console.log(dwight);

console.log(students.length);

Adding to array:

students[4] = 'Bishal';
students[10] = 'Marcus'; <- will show undefined up to 10
students[0] = 'Tanesha'; <-- re-assigns the value

console.log(students)

// most common way to add to the end of the array using .push() method

students.push('Steve');

console.log(students);

// add to beginning of the array using .unshift(); adding to beginning will take up more time, especially if the array is big

students.unshift('Ella'); <--- makes Ella 0

console.log(students);

// add to the middle/or other spots in the array .splice()
// parameters - what index to start, # of items remove, what to add

students.splice(3, 0, 'Ryan'); <-- 0 tells it you're not removing naything

console.table(students)

students.splice(2, 2,'Ryan') <-- first number, the middle number is HOW MANY items you're removing if any, and then what to add

### CSS

#### Box Model

<header>
  <div> class="divOne">Div One</div>  **ids take precedent over styling**
  <div> id="divTwo">Div Two</div>
  <div>Div Three</div>

  Centering text:
   text-align: center;
  **Font size: vw adjusts size with the size of the page "scale"**
  width: max-content;
  margin: 50px auto; <- feeding two values will give it vertical & horizontal

.divOne {
  background-color:
}

#divTwo {

}

class has a period .
id is a number #

#### For Loops

- great for doing something a certain amount of times
- great for iterating/ over/through arrays
- anatomy of a for loop

  - for(starting value; condition; increment){
      code block -- do something each iteration
  }

let students = ['thomas', 'eden', 'ella'];

for(let i = 0; i < students.length; i++) {
  console.log('Hey! ${students[i]}!');
  if(students[i] === 'Steve'){
    console.log('Hey whats up Steve!');
    }
  }

  1st iteration - i = 0, i < 22 (true);
  console.log('Hey! ${students[0]!'};)
  i gets incremented
  2nd iteration - i = 1, i < 22 (true);
  console.log('Hey! ${students[0]!'};)
  i gets incremented
  3rd iteration - i = 2, i < 22 (true);
  console.log('Hey! ${students[0]!'};)

  starting at back of array:
  for(let i = students.length-1; i >= 0; i--) {
console.log('Hey! ${students[i]}!')

break; will break out of for loop and stop when it reaches value.

#### While Loops

- Great for doing something however many times you need until a condition goes false
- notorious for getting stuck in infinite loops
- anatomy of a while loop

while(condition){
  do something until condition is false
}

let myNumber = 4;
let userNumber = prompt('What number am I thinking of?')

while(userNumber != myNumber){
  userNumber = prompt('What number am I thinking of?);
  if(userNumber == myNumber){
    alert('you are correct!');
  }
}

let students = ['thomas', 'eden', 'ella'];

         20       &&.  true
while(clueGuesses && !foundSuspect){
  let myGuess = getRandomStudent();
  console.log(`it was ${myGuess}, in Remo, with the candlestick! Guesses: ${clueGuesses}`);
  clueGuesses--;
  if(myGuess === suspect){
    foundSuspect = true
  }
}

### Lab 03

- 