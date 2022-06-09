# Class 38

## Code Challenge

```{python}
let array = ["chicken","egg","green tomatoes"]
const arrays = array.map(item => {
    return "fried " + item
})

console.log(arrays)
```

## Lab

- index.js is appropriate place to manage state
- state passed into components this way 
- count={questions.length}
- onQuestion={handleQuestion}
- answer={getAnswer()}
- questions={questions}

- index.js deligates to somewhwere else but keeps what is most approporate for it
- mainting state
- modifying state as needed

- work top to bottom

- Header
  - component of a page
  - put in components folder
  
```{js}
export default function Header(){
  return (
    <h1>
    hello
    </h1>
  )
}

```

- import into index
- put header in div
- build up components 
- 