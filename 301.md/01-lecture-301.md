# Review

```js

// Hoisting

// vanilla JS function declaration
let sum = add(2, 3); // if this were myAdd it wouldn't work because you can't invoke mrthod before declared
console.log(sum);

function add(a, b) {
  return a + b;
}

// vanilla JS function expression
let myAdd = function(a, b) {
  return a + b;
};

// Arrow functions

let arrowAdd = (a, b) => { // need parens because it has more than 1 parameter
  return a +b;
};

let arrowAdd = a => {
  this // this doesn't mean the function itself
  return a + 6;
};

// Classes

// vanilla constructor
function CountryState(name, capital) {
  this.name = name;
  this.capital = capital;
  this.isAmazing = true;
}

let washington = new CountryState('Washington', 'Olympia');
console.log(washington)

// as a class

class CountryEntity {
  constructor(name, capital) {
    this.name = name;
    this.capital = capital;
  }
  awesome = () => {
    console.log('I\`m awesome');
  }
}

let classWashington = new CountryEntity('Washington', 'Olympia');
console.log(classWashington);

class Province extends CountryEntity {
  constructor(name, capital, premier) {
    super(name, capital);
    this.premier = premier;
  }
  wow = () => {
    console.log('wow');
  }
}

let britishColumbia = new Province('British Columbia', 'Victoria', 'John Horgan');
console.log(britishColumbia);

britishColumbia.wow();
britishColumbia.awesome();

classWashington.awesome();
classWashington.wow();// only BC can you wow

// For Each

let array = [1, 2, 3];
let newArray = [];

array.forEach((element) => {
  newArray.push(element + 1); //++ doesn't work in arrow functions!
});

console.log(newArray); // will return [2, 3, 4]
```

## React 

- a JS library that we can use to help us build user interfaces
- UI components: what gets passed to you when you open a web page.
- individual components that make up our pages
- as developers we don't like to repeat ourselves
- using different words, but using name html tags and styles
- use JS to build components and give it different content
- not as much DOM manipulation!
- nodes. package manager to build react components
  - necesarry to use react and build servers
  - terminal command: npx
- react has to be compiled for the browser to understand it
- npm start will act as live server and open it in console
- building app.js from scratch!
- netlify to deploy site

``` js

import React from 'react';
    class App extends React.Component{
  render() {
    return (
      <>
       <Header></Header>
          <main>
            <article>
              <h3>Ella</h3>
              <p>text goes here</>
            </article>
          </main>
         <footer>
          &copy, Code Fellows, 2022
         </footer>
      </>
    );
  }
}

export default App;
// React cam only return this code if it's wrapped inside it's parents element
// in src folder create a Header.js file
// all js files should have import React from 'react';

class Header extends React.Component {
  render() {
    return (
      <header>
        <h1>People of 301D83</h1>
      </header>
    )
  }
};

class Main extends React.Component {
  render() {
    console.log(this.props.name);
    return (
      <main>
       <Person 
       name="Ella" 
       hometown="Ventura" 
       hairColor="brown"
       /> 
       <Person name="Name">
       <Person name="Name"/>
      </main>

    )
  }
};

// Props
// cannot change the value of a prop

