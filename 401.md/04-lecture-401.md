# Class 4

## Code Review Lab

## Code Review Code Challenge

- base case is when youre done recursing
- search is done and you won't find value
- BigO Sapce is Log N as well
  - the recursion goes to the call stack
  - it stacks up and is related to it being logN
- Think about the places where the code will break
- think about the questions to clarify how you will solve the problem
- think about the kinds of tests you would really write

- ALWAYS ASK FOR EXAMPLES

- fibonacci sequence formula in python: ((((1+math.sqrt(5))/2)**n-((1-math.sqrt(5))/2)**n)/math.sqrt(5))

## Classes

```{python}
<!-- test -->

def text_boxer_create():
    assert Boxer()

def text_boxer_name():
marv = Boxer("Marv")
actual = marv.name
expected = "Marv"
assert actual == expected

def_text_boxer_greet(marv):
actual = marv.greet()
expected = "The name's Marv"


<!-- .py -->

<!-- define super class above other class -->

class Dog:

all_dog_count = 0

@classmethod
def get_all_dog_count(cls)
  return cls.all_dog_count

  def __init__(self, name="unknown"):
  self.name = name
  Dog.all_dog_count += 1

    def sleep(self)"
  return "zzz"


class Boxer(Dog):

  pre_breed_count = 0

    def __init__(self, name="unknown"):
    Boxer.count += 1
    super().__init__(name)

  def greet(self):
    return f"The name's {self.name}"

  @staticmethod
  def get_characteristics():
  return "boxers are lovers not fighters"



class Puggle(Dog):

  count = 0

  def __init__(self, name="unknown"):
    Puggle.count += 1
    super().__init__(name)

  def greet(self):
  return f"I am {Lela}"  

  @staticmethod
  def get_characteristis()
  return "like a mini boxer"
  <!-- this is not tied to particular instance -->

  @classmethod
  def get_breed_count(cls):
  return cls.per_breed_count


```
