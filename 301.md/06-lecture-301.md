# Lecture

## WRRC

- difference between front end and back end
  - front end is our computer
  - back end is someone elses computer
  - i order my food at the table (front end), and they make it in the kitchen and send it out to me (back end)
  - a computer that us accessing another computer

## Rest

- Representational state transfer
  - Get: this is what were are using this week
  - Post
  - Delete
  - Put

## Anatomy of a URL

- ? notes the beginning of query
- key = key value pair
- & notes another set of key-value pairs/ parameters
- query string inside a URL is called a parameter

## Axios

- npm package
- npm is node package manager
- a package is someone else's code that we can use
- npm i axios
  - installs axios
- you will see it in json
- import axios from 'axios';
- add async
- add await

- in event handler set variable to what you want to get returned. 
- *json formatter extension for chrome!*

``` js
let starWarsCharacter = axios.get(/*paste url of data here*/);
```

- we want to get the data into state
- working with axios we need to use the word data!!
- react needs a KEY to track each item
- you can use index as a key

## Lab 6

- if running API you don't want to give data away without aauthentication oor charge
- Some sites will cut you off if you request too much data
- API key is access token

- LocationIQ
- Login/create
- gives you free API key
- API key is like credit card number
- Authorized HTTP references
  - localhost
  - netlify
  - url to site
- API key goes in root in .env file (sibling of gitignore)
- #environment in git ignore
  - .env
- sample.env
  - untracked by git
- .env
  - REACT_APP_LOCATIONIQ_API_KEY
  *set to key value*

- async is passed because it's going through a lot of data
- letting JS know it could take time
- 