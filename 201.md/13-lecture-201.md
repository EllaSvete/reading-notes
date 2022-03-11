# Class 13 

## Data Persistance

- local storage
  - an obbjext stored in a browser application
  - local storage is specific to the one computer
  - no expiration

- Database
  - SQL - postgres(401)
  - NoSQL - mogodb(301)

## Why

- So users can retain data between page refreshes or accessing different part of the application

## How it is stored

- JSON - JavaScript Object Notation
  - text based, arrays, other data
  - key: value pair
  - to stringify our objects using a method `JSON.stringify()`
    - pass in object to stringify

### Methods on our Local Storage Object

- `getItem(key)`
- `setItem(key, value)`
- `clear()`
- `removeItem(key)`

- `localStorage.getItem(key)`

### Steps

- to put something into storage
  - `let stringifiedItems = JSON.stringify(myObj)`;
  - when we stringify the objects/data, it changes, it strip any reference to our constructor away
  - `localStorage.setItems(`myStuff`, stringifiedItems);`
- to get it out of loval storag
  - `let stuffImGettingOut = localStorage.getIrm(`myStuff`);`
  - `let parsedStuff