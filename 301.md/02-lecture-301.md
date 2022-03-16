# Lecture DAy 2

## Code Review

- export default App: needs to know what it needs to grab
  - two parts:
    - App is getting imported
    - and then it must be exported
- render is expecting to see single statement
  - wrapping it in a div makes render *think* its a single statement

### Code Challenge: Map

- Two kinds of Map in JS.
  - will be using Map Array method
- look up DM

- Parameters callbackFn
- Map has a return value
  - map creates and returns a new array
  - we to figure out what goes in the array

```js

let arr = [1,2,3];
let stringArr = ['one', 'two', 'three'];

let newArr = arr.map((num) => {
  return num * 5;
});
console.log(newArr);

let newStringArray = stringArr.map(str = > str.toUpperCase());

console.log(newStringArray);

```

## Lab Demo

- data.json: does not need export because it's not a component

``` js
// App.js:

import data from './data.json';
// all images/name/info will go in this file

<Main
  data={data}
  />

//Main.js:
render() {
  console.log(this.props.data);
  let people = [];
  this.props.data.forEach((person, index) =>{
    people.push(
      <Person
        name={person.name}
        imgUrl={person.imageUrl}
      />
    )
  })

  return (
    <main>
    {people}
    </main>
  )
};
```

- State is data that belongs to a specific component
- "liking" a post should be stored in particular instance of that data
  - info can change
- We will need event handlers so it knows when and how to change the dtata
  - what caused the change
- props: component cannot change the value
- state: data is owned my particular component and is stored there
- we will add state to people to show how mnay times they have been greeted

```js
// in each Person component

class Person extends React.Component{
  constructor(props){
    super(props);
    this.state = {
      waves: 0
      needsHelp: false,
    }
  }

handleWaves = () => {
  this.setState({ 
    waves: this.state.waves + 1
    // banana: 'banana' you can create a variable
  });
};
needsHelp = () => {
  
}

  render() {  
    console.log(this.state);
    return (
      <article>
        <h3>{this.props.name}</h3>
        <p>{this.states.wave} greetings</p>
        <p onClick={this.handleWaves}>Say hello!</p>
      </article>

    );
  }
}

``` css
Header.css //import to Header.js

h1 {
  font-size: 5vw;

}

Main.css

main {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around
}

Person.css

article {
  border: 
  padding: 1vw;
  margin-bottom: 1vw;
  width: 16%;
}

article p: last of type {
  padding: left 1rem;
  cursor: pointer

}

article p: last-of-type {

}

- Bootstrap uses components already built in. 
- Adding Bootstrap

- npm install react-bootstrap and reg bootstrap
- import css at root in index or App
  - index is better, out of side out of mind
  - import before other css

- Button
  - in person component
  - import Button from bootstrap before other css files
- thne you can pu tbutton into code

``` js
<button>Regular BUtton</> // html button is a form component

<div>{this.state.needHelp ? 'I need Help' : ''}</div>
<Button 
  className="article-button"
  onClick={this.needsHelp}
>
  I need help
</Button>

// style button is Person.css file

.article-button {
  margin: .2rem .1vw;
}

// Ternary
// WTF
// What ? True: False

let unicorns = true;

unicorns ? console.log('wow') :
console.log('no way!');
