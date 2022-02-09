# Day 2 Lecture Notes

## Lab 2 code review

- header: this is where links could go, like for nav, or list, anchor tag, h1, header image
- inline style often makes your html look messy
- html using double quotes to encapsulate "background-color"
- option+shift+f will format file and get everything where it needs to be.
- what are you doing in () you are doing string cancadenation
- template literal:
  alert(`welcome to the thunderdome ${responseOne}!!!`);
  - purpose of this is to bring in variable - use only then!
  \' to use apostrophe 

## Data Types

- JS A way or organizing and labeling our data
- format data that our program can anticipate and use properly

JavaScript is a **loosely typed** and **dynamic** language

- Loosely typed meaning we don't have to know the type of data to declare a variable.
- Variables do not need to be declare with a type

`let cat;` is a variable you could reuse somewhere in the file

- Dynamic meaning I can change the type of data after the variable has been declared.

`cat = 3;`

`cat = 'cuddly';`

`cat = false;`

- const keeps our variable a certain data type. const dog = 'woof';

### Numbers

- `4` `1.24` `-200`

### Strings

- notated with `''` single notes
- single quotes in javascript for readability
- `'hello'` `'4'`

### Booleans

- `true` or `false`

### Undefined

- something that dos not yet have a definition

### Null

- defined as none
  - undefined will throw un error, null will not because it is defined as "nothing"

## Conditionals

- If/Else

- if something evaluates true, do something 

if(somethingEvaluatesTRue){
  do something -- code block;
} else if(somethingEvaluatesTrue){
  do something -- code block;
} else{
  do something -- code block;
}

'use strict'; means use strict JS tools

let isTrue = true;
let isFalse = false;

if(isFalse){
  console.log('this code ran!');
} else if(isTrue) {
  console.log('nah girl this code ran!');
} else { <-- if nothing else, do this. no condition
  console.log('This one ran!!')
}

- Shortcut: hold option and arrow key and it will move your line of code.

## Comparison Operators

- == comparative "loosely equals"" - NOT OUR WORLD
- != "loose inequality"
- < less than <=
- > greater than >=
- === strict equals - THIS IS OUR WORLD
- !== strict inequality

let a = 5;
console.log(a <10); <--- this will give us our Boolean value: true

if(a > 3){
  console.log('true!;);
} else if(a < 10) {
  console.log('this is also true!');
} else {
  console.log('that was false')
}

## Logical Operators

- && - and
- || - or
- ! - not

if(isTrue || isFalse) { <-- true OR false, wont run with &&
  console.log('will this run');
}

if(isTrue || !isFalse) { <-- the ! will automatically give you the opposite
  console.log('will this run');
}

//
if(response === 'yes' || response === 'y'){

}

## Git - GitHub

- git: Version Control - software on our local machines
  - track changes we make through series of commits and branches
- GitHub: a website - stores our code so we can share and collaborate amongst teams **we use git on our local machines to send those changes to GitHub**
- gitflow:
  A: add
  C: commit
  P: push

- only work on local device NOT github  
- git clone < https url> OR < SSH>
- git push origin main or < branchname>