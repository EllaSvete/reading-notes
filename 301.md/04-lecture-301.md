# Class Notes

``` js

let starRatings=[1,2,3,5,6,7,8,9,10]; ///

class App extends React.Component {
  constructor(props){
    super(props);
    this.state: {
      name: "Thing to Rate",
      starRatings:
    }
  }



handleName = (event) => {
  this.setState({
    name: event.target.value;
  });
};

handleSelect = (e) => {
  let selected = e.target.value;

  if(selected === 'even'){
    let newStars = starRatings.filter(num => num % 2 === 0)
    this.setState({starRatings: newStars});
} else if (selected ==='odd'){
    let newStars = starRatings.filter(num => %2 !== 0);
    this.setState({starRatings: newStars});

} else if { //ALL
this.setState({starRatings: newStars});

}

render(){
  return(
    let listItems = this.state.starRatings.map(item, index) =>{
      return <li key={index}>{items}</li>
    })
<>
<header>
<h1>You're a star</h1>
</header>
<form>
  <fieldset>
    <legend>Form</legend>
    <label>Name
      <input type="text" onInput={this.handleName}/>
    </label>
    <label htmlFor="numberOfStars">How Many Stars</label>
    <input id="numberOfStars" type="number" onChange={this.handleStars}/>
  </fieldset>
  <fieldset>
  <legend>Track Ratings</legend>
  <select>
  <option value="all">All</option>
  <option value="even">Even</option>
  <option value="odd">Odd<option>
  </select>
  </fieldset>
  </>
  )
}
```

- invalid DOM property: use htmlFor instead of for because it confusing javascript-
- sort list by odds and evens, 
- things to have in handle submit 
  - handleSubmit = (event) =. {
    event.preventDefault
  }

- Bootstrap component:
  - npm install 
  - import component we want to use
  - import minified styles

import forms and button

``` js
<Form onSubmit={this.handleSubmit}>
  <Form.Group>
    <Form.Label>
    </Form.Label>
      <Form.Control
        type="text"
        onInput={this.handleName}
      />
  </Form.Group>
    <Form.Group>
    <Form.Label>How many Strars
    </Form.Label>
      <Form.Control
        type="text"
        onInput={this.handleStars}
      />

  <Button>submit</Button>
</Form>


```