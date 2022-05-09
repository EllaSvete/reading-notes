# Class 15 TRees

- tree node is a component that contains its own values
- contains references to other nodes

- Working with a binary tree

- every node in the tree is a fork in the road
- you can go either way but be consistent
- left first USUALLY
- what is nothing is to the left?
- go right, and see if something is there
- if 3 is sum on the way in
- and the ride node is 4
- total is 7
- keep left and stay consistent
- once its done
- has the root node done its job?
  - yes because it checked left first

- 3 things
  - adding sum
  - check left
  - check right

- notice when something is being done the same way each time
- do soemthing repeatedly while keeping track of things

- you could use a loop
- you can use functions to carry out steps and return values
- functions are good at calling themselves
  - keep track of where we are along the way
- traverse()
  - add sum
  - go left - traverse() on the left
  - go right

- reason to stop recursing is the base case
  - function will exit
  - will retrun the sum as you traverse
  - function call stack keeps track for us

- recursion and trees will give you nice lean code and you wont have to keep track of the loop

- 