# Class 07 Lecture Notes

## constructors

### what are they?

- a special type of function
  - start with keyword 'function'
  - acts like a lueprint/'factory' for objects
  - instantiate objects for us

  ### why

  - keeps code try
  - prevent bugs

  - inherits

``` javascript

'use strict';

 // capital letter! anything capital in sJS IS CONSTRUCTOR OR CLASS
 // parameters - unique properties

 // table:

 let table = document.querySelector('table');

 // go into render and write note 
 //table render to DOM

 let row1 = document.createElement('tr')
 table.appendChild(row1);

function students(name, pronouns,){
  // this refers to the object that will be instantiated
  this.studentName = name;
  this.Pronouns = pronouns;
  this.currentClass = '201d83';
  this.optional = [];

  students.push(this);
}

// instantiate a new student
let christopher = new Student('Christopher', 'he/him');
let katrina = new Student('Katrina, 'she/her');
new Student('Michelle', 'she,her');


christopher.optional.push(1,2,3)


Students.prototypes.greetsClass = function(){
  this.greetsClass = function(){
    console.log(`Hello ${this.currentClass}! I'm ${this.studentName}`);
  }
}
console.log(students)

christopher.greetsClass();

Array.prototype.doSomething = function(){
  console.log('I made this array do something!');
}
students.doSomething();

//REFACTORING LAB

// ***** constructor *******

function Kitten(name, interests, isGoodWithCats, isGoodWithDogs, is Good With Kids, photo){
  this.name = name;
  this.interests = interests;
  this.isGOodWithCats = isGoodWithCats;
  this.isGoodWithDogs = isGoodWithDogs;
  this.photo = photo;
  this.age = 0;

  kittenCaboodle.push(this); //this is pushing all of my instantiated objects into an array
}

Kitten.prototype.getGAge = function(){
 this.age = `${randomAge(3,12)} months`;
}

new Kitten('Frankie', ['wet food, 'fish toys'] , tru, false, true, 'img/frankie.jpeg');

console.log(kittenCaboodle);

//compare stores, see whats unique : min max, average, location.
```
