# Lecture Day 3

## Code Review

## Code Challenge

## Lab Demo

- The Problem 
  - changing a parent element from child
  - use App.js and find shared element

- We will be changing the header
  - we want to pass it as a prop

```js

//App.js

class App extends React.Component {
  constructor(props){
    super(props);
    this.state = {
      hearts: '',
    };
  }
}
addHearts = () => { // arrow function inherit context under which they are declared
  this.setState({
    hearts: this.state.hearts + 'heart emoji'
  })
}
render() {
  return (
<Header
  hearts={this.state.hearts}
/>
<Main
addHearts={this.addHearts}
/>
  );
}

//Person.js
<img
onClick={this.props.addHearts}
>

```

- adding state to og child
- state modifies value that the parent is reading
- parent checks state and passes prop to component
- App. js has event handler
- HornedBeast.js gas event listener
- then pass reference from handler to listener
- when onClick happens its referring to handler on App.js

## Lab 03

- adding Modal to Gallery of Horns

- a Modal is a pop up window that is contained within browser window
  - shows up within context of screen
  - removal of scroll aspect

- import data.json file into your App component that sends data into Main

- use Map for jason data

- send function into main to update state in the app

- create SelectedBeast component in App
  - this will be the Modal
- Bootstrap modal comes wih x button