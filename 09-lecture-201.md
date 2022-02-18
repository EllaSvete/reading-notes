# Class 9 lecture

#### types

- click
- submit- keypress
- hover
- mouseover
- page load

### javascript - code: event listener

- code that gets a trigger when our even has been fired
- target an html element to lsiten to

```js
let myContainer = document.getElementById('container')
```

- specify what type of even to listen
- specify what to do when we hear the event (event handler= callBackFunction)

```js
myContainer.addEventListener('click, callBackFunction)
```

### Javascript code: event listener

- callback function: function that is entered as a parameter of ANOTHER function/method

```js
function handleClick(event){
  console.log('i\'ve been clicked!');
}
```

```html

<form id="my-form">
  <fieldset>
    <legend>Gives your fieldset some content</legend>
<!-- one way for inputs and labels ***for on label must match id on input**** -->
    <label ="name"></label>
    <input type="text" name="fullName" id="name"> //name if how you target something
<!-- event.target.fullName.value -->
      <label>Age
        <input type="number" name="age" required> // could be "password" too
  <!-- event.target.age.value -->
       </label>

        <label for="housewives">Fave housewives franchise?</label>
        <select name="housewives" id="housewives">
          <option value="slc">SLC</option>
          <option value ="bevHills">Beverly Hills</option>
          <option value="none">None</option>
        </select>

  </fieldset>  // can have multiple within a form "address" "name" a way tp organize
  <button type="submit">Submit</button>
</form>

```

```js

// step one - grab the element to listen to
let myform = document.getElementById('my-form');

//step 3 event handler
function handleSubmit(event){
event.preventDefault();
console.log('submit');

let name = event.target.fullname.value;

let age = +event.target.age.value;
console.log('age',age);
console.log(typeof age);

}


//step 2 - attached your event listener to your elemt and tell it what to listen tfor and pass in our Event Handler (callback function)

myform.addEventListener('submit', handleSubmit);


/// split is a string methos that will split on the character provided. it will return an array of elements that were sokuts, 

// lab:
// adding a store that is going to feed your table
// the info from constructor is going to inform what is in the store
// make sure you're calling what needs to be added
// build form in sales.html
// re-render foot because it wont automatically update totals
// numbers for new store are made up
//remove element and call stand alone function for footer

let newKitten = new Kitten(name, interests, isGoodWithCats, isGoodWithDogs, isGoodWithKids, photo);

newKitten.getAge();
newKitten.render();

kittenForm,reset();//not needed, but the information will sit there without it.
