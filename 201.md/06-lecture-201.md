# Class 06 lecture notes

## Objects

### What are they?

- data type
- comma separated key/value pairs- wrapped in curly braces
- like arrays group data, or functions
  - in objects functions are referred to as Methods

  ```javascript

  let personArray = ('Audrey', 35, 'instructor', true)

  let audrey = {
    name: 'Audrey',
    role: 'instructor',
    age: 35,
    isRemote: true
  }
  ```

  'use strict';
  let audrey = {
    name: 'Audrey',
    position: 'instructor',
    age: 35,
    course: '201d83',
    says: function(){ <--- is method!
      console.log('You can do it!')
    }
    10: 10000,
  }

  // get the name out of the object
  // DOT NOTATION = object.key

  console.log(audrey.name);
  console.log(audrey.age);

  // BRACKET NOTATION = obj['key'] they key name needs to be a string
  console.log(audrey['course']);

  // DOT notation is most commonly used.

  // calling my methods outside of my object
  audrey.says();
 
  // add properties outside of object
  audrey.interests = ['art', 'celebs', 'sleeping;]

  console.log(audrey);
  
  audrey.advises = function(){
    console.log('Get help after 15 minutes');
  }

  audrey.advises();

//

  let audrey = {
    name: 'Audrey',
    position: 'instructor',
    age: 35,
    course: '201d83',
    says: function(){ <--- is method!
      console.log('You can do it!')
    }
    classIntro: function(){
      console.log(`Hello, ${this.course}`);
      <!-- console.log(`Hello, ${audrey.course}`); -->
      <!-- "this" refers to where it's located so it will have different meanings. refers to the object you are in. -->
    }
  }

  audrey.classIntro()

### Demo

1. window into DOM
2. 
