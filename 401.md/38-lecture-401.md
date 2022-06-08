# Class 38 Notes

- Conditional rendering
  - use if or the conidtion operator to create elements representing the current state

- Element variables
  - this can help render a part of the component while the rest of the output doesn't change
  - have state for logged in and logged out
- embed JSX expressions by wrapping in curly braces
- includes logical && operator
- true && expressiona always evaluate to expression
- false && expression evaluates to false
- if the condition is true the element after will appear in the output
- if false react will ignore and skip
- ternary:

```{js}
render() {
  const isLoggedIn = this.state.isLoggedIn;
  return (
    <div>
      The user is <b>{isLoggedIn ? 'currently' : 'not'}</b> logged in.
    </div>
  );
}
```

```{js}
render() {
  const isLoggedIn = this.state.isLoggedIn;
  return (
    <div>
      {isLoggedIn
        ? <LogoutButton onClick={this.handleLogoutClick} />
        : <LoginButton onClick={this.handleLoginClick} />
      }
    </div>
  );
}
```

- Preventing component from rendering
  - RETURN NULL INSTEAD OF RENDER OUTPUT

- Lists and Keys
  - map() to take in array

- Rendering Multiple Compoenents

```{js}
function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    <li key={number.toString()}>
      {number}
    </li>
  );
  return (
    <ul>{listItems}</ul>
  );
}
```

- Keys

  - identity which items have changed been added, or are removed
  - use id from your data as key
  - try to not sure index
  - keys only make sense in the context of the surrounding array
  - keys must be unique
  - they don't get passed to components

- [Forms](https://reactjs.org/docs/forms.html)

- [Lifting State](https://reactjs.org/docs/lifting-state-up.html)

- Composition Vs Inheritance

- Containment
  - some components don't know their children ahead of time
  - use special children prop to pass children directly to output

```{js}
function FancyBorder(props) {
  return (
    <div className={'FancyBorder FancyBorder-' + props.color}>
      {props.children}
    </div>
  );
}
```

- Thinking in React
  - use the same technqiues to build components as deciding if yuo should create a new function or object
    - single responsibility principle
  - if model was built correctly, your UI will map nicely.
  - idenitify components
  - arrange into hierarchy
  - build static version
    - state is reserved for interactivity
  - identify minimal representation of the UI state
  - lastly, identify where state should live.