# Class 37

## Code Challenge

- a leaf node is a node without any children

## REACT, Tailwind, NEXT.js

- npx create-next-app app-name (hiphens)
- cd into project
- npm run dev

- start in pages index.js
  - delete things in the Home Component!
  - something renderable gets returned in functional component

-tailwindcss.com

- tailwind config
  - rpeaplce module exports

- globals.css

- back in functional Component
  - <header className="py-6 px-8 bg-gray-500"></header>
      <h1 className="text=4xl text-gray-50"></h1>

- command k
  - search what you were looking for

- function Footer(props){
  return <footer className="bg-gray-500 py-6 px-8">
      <p className="text-gray-50">&copy;{props.copyright}</p>
}

- build out skeleton of components
- w is for width
- w-1/2
- flex flex-col items-center

- return <form onSumit={props.onSubmit} className="flex w-1/2 p-2 big-gray-200">
  <input className="flex-auto pl-2" placeholder="enter here.." required/>
  <button className="px-4 py-2">Ask</button>

- passing props.. find the parents
- pass the props where needed
return outter dive
- <div classname="w-96 h-96 bg-gray-900 rounded-full">
    <div className="w-56 h-56 bg-white rounded=full relative top-16 left-8 flex items-center justify-center">
    <p>{props.question}</p>
    </div>
</div>

- import (useState) from 'react'
- const [question, setQuestion] = useState("enter here...")