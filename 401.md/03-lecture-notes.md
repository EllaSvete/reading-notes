# Class 3: FileO and Exceptions

## Code Review:

- :middle_idx is middle idx and to the right
- :middle_idx is middle idx to the left
- python lists are laid out in continuouis segments of memory

```{python}
veggies = ["artichoke", "brocoli", "cucumber", "daikon"]
fruits = ["apple", "banana", "cherry", "date", "strawberry"]

def find_insert_index(items):

<!-- length of 4 should result in 2 -->
<!-- length of 5 should result in 3 -->

<!-- position = int(-(-position//1)) -->

if len(items) % 2 == 0:
  insert_index = len(items)// 2

else:
  insert_index = len(items)// 2 + 1

return insert_index

assert find_insert_index(veggies) == 2
assert find_insert_index(fruits) == 3

print("TESTS PASSED)
```

```{python}

length = len(items)

insert_index = length // 2 if length % 2 == 0 else length // 2 + 1

```

```{python}

insert_index = -(-length // 2)

```

- floor division (//) outputs a integer

```{python}

insert_index = (length + 1) // 2
<!-- 4 + 1 //2 = 2, 5+1 // 2 == 3 -->

```

## Today's code challenge

- Binary search
  - sorted 1 demensional array
- use python naming conventions
- when something isn't in the list
  - -1 returned
- for efficiency
  - Binary Search

## LAB 3

- print(*my_list)
  - prints arguments separately in the list
- my_string = "Hi from {}"

- todays lab is a command line interface
- we're not testing print and input functions
- tests are given to US
- tuple will guarantee the list will not be changed
- tuples and lists can be unpacked
  - first_value, second_value = my_tuple

## DEMO

- open(file.txt)
- read(file.txt)
- dir(file.txt)

- try except to handle errors
- have specific errors your catching for
- dividing by wrong type
  - except when there is an exception
    - same as except with nothing else
- finally is run no matter what
- last thing after a try except
- Try to use a built in error, and exception types

- Todays lab handle incorrect path to template
- 