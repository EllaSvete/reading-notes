# Lecture

## Getting started

- setting up own server to run as API
- Node
- NPM
- Express.js - npm used to build a server\
- create git repo
- clone it down
- npm init (installs node in project)
- this is setting up json data
- server.js instead of index.js
- cp config-files/.gitignore -> into new folder
- cp config-files/.eslintrc.json -> new file
- cd in to file, the copied files should be in there
- needing a entry point file.
- touch server.js
- code .
- empty server.js file
  - you'll need window with server code and front end code
- server file

- npm i express : installs express
- npm i dotenv

```js
'use strict';

console.log('My first server'); // this will log in terminal

//REQUIRE
// in our servers, we have to use 'require' istead of import. here we will list the requirements for server
const express = require('express');
require('dotenv').config();
let data = require('./data/pets.json');

//USE
// once we have required something, we have to use it. this is where we assign the required field a variable. React does this in one step with "import" express takes 2 steps: "require" and "use"
const app = express();

// define PORT and validate that .env file is working
const PORT = process.env.PORT || 3002;
// if my server is running on 3002, I know something is wrong with my .env file or how I'm importing the values from it.

//ROUTES
// we will write our endpoints here
//app.get() correlate with axios.get
app.get('/',(req, response) => {
  response.send('hello, from our server!');
});

app.get('/pet', (req, res) => {
  let species = req.query.species;
  let petObject = data.find(pet => data.species === species);
  let selectedPet = new Pet(petObject);
  console.log(species);
  re.send(selectedPet);
})

app.get('*', (request, response) => {
  response.send('Page does not exist.')
});

//ERRORS
//handle errors

// CLASSES
class Pet {
  constructor(petObject) {
    this.name = petObject.name
    this.species = petObject.species
  }
}

//LISTEN
// start the server
//listen is an Express method that takes in a port value and a callback
app.listen(PORT, () => console.log(`listening on port ${port}`));

```

``` js
// in env file
PORT=3001
```

- anytime you make changes to server code you have to restart server app
- npm i -g nodemon installs autoserver restart
- nodemon instead of npm start
- npm kill-port 3001 kills whatever process is running

- deployment
  - git status
  - git add .
  - git commit -m 
  - git push

- Heroku
  - new app
  - city-explorer-301svete
  - usa
  - no pipleline
  - create app
  - connect to repo on github
