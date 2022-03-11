# class 12

let randomIndexes = []

function renderImgs(){

``` js

while (randomIndexes.length < 3){
  let randoNum = getRandomImg();
  while(!randomIndexes.includes(randoNum)){ // checking to see if randoNum is not in array
  // includes returns a boolean
    randomIndexes.push(randoNum);
  }
}

let itemOne = getRandomImg();
let itemTwo = getRadnomImg();
let itemThree = getRandomImg();

```
