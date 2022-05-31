# Lecture Hashtables

- Hastables are used to determine index of array
- buckets: what is contained in each index of the array
- collision: what happens when one or more key gets hashed to same location of the hashtable
  - collisions can be resolved

- key would know how to find the right spot
- how would the key find the index  its looking for?
- key if often a string, or something hashable
- something that will turn string into an index
  - run funciton on key 
  - hashfunction!
- a hashcode codes the key into a integers
- key always has to equal the same value ALWAYS
- hashtable is created from an array
- size 1024 is common
- need someway to generate a key:

- add or multiply ASCII values
- multiply by prime number such as 599
- use modulo to get remainder or results when divided by size of array 
  - stays in range
- insert into the array at that index

- if the index is a linked list
- with multiple things, how do you know which thing to grab?

- when you put things intp the appropriate array location, keep track of the key!
- got through whoever is in unit and compare the key to other keys in the array(LL)
- you would traverse it by checking the next values

- ascii numbers:

```{python}
        ascii_values = [ord(letter) for letter in string]
        return sum(ascii_values)
```



