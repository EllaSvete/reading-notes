# Class 2: Modules and Recursion & Big O

## Code Challenge Review

- first argument that is a string, is the prompt which is optional.
  - it will show to the user
  - it will store it in the input array
  - instead of camel case use snake_case

- Pep 8
  - guidelines and best practices for Python
- Class names should use CapWord
- functions and methods use snake_case

## Today's Code Challenge

- Whiteboard only
- takes an array, and a value to be added
- return array with new value added to the middle index
- return same array, altered

## Big O

- Time & space scaling over time depending on input size
- def add(xy) 1+2 is flat
- different ways number of operations and memory scales depending on input size
- there is a measurement for how memory scales depending on input size

## Lab Review

- """ """ you can put a whole string and it ill add spaces
- whole_menu = appetizers + entrees + desserts

- false-y things equals: False, 0, '', 0.0, None
- .title will change the it to be capitalized
- the difference is that the code always checks to see if an 'if' statement is true, checks 'elif' statements only if each 'if' and 'elif' statement above it is false, and 'else' runs only when the conditions for all attached 'if' and 'elif' statements are false.

## Test Driven Development

- source .venv/bin/activate
- pytest
- mkdir fizz-buzzz
- cd fizz-buzz
- touch fizz_buzz.py
- touch tests
- rm tests
- mkdir tests
- touch tests/test_fizz_buzz.py
- touch tests/__init__.py
- python3 -m venv .venv
- source .venv/bin/activate

- pytest is not part of python library
- pip install pytest
- oh you must install when you're in you're folder!!
- pip freeze > requirements. txt
- cat requirements.txt
  - shows contents of the file
- pip install -r requirements.text
- requirements.text should be in github repo!
- not .venv
- they install libs in reqs

```{python}
def test_fizz_buzz_one()
actual = fizz_buzz(1) /*need fizz_buzz function in module*/
expected = '1'
assert actual == expected
```

- module is a file

```{python}
def fizz_buzz()
pass /*pass lets you have a function with nothing in it*/
```

- import module into test
- from fizz_buzz import fizz_buzz
- pytest runs test
- fizz_buzz() module is required to have a positional argument

- TDD want you to take baby steps to pass test
- pass the test

- if num % 3
- % checks the remainder

- print will not test
  - it's not returning something!

- refactoring without unit tests is just moving shit around
- with unit tests makes you feel secured you're not breaking anything

- package in python is a folder than contains modules
- a module is a file that contains python definitions
- packages can be nested
- __init__py is at top level of test folder
- recursion package you import factorial
- 3*2*1 is still 6
- facotiral is the product of numbers

- looking at something one at a time, 
- skipping test
- right above function line you want to skip
- @pytest.mark.skip("pending")

- what we want is some number * factorial of smaller number

```{}
if n <= 1:
return 1


return n * factorial(n-1)
```
