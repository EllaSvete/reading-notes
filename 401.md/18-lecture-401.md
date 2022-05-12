# Class 18

- how do you keep track of a nodes children?

- start a root and add it to queue
- enqueue and then dequeue

- now what?

- when it gets dequeued, go through children and enqueue children
- dequeue from front
- and then look at the left child's children
- level search
- check list of children instead of left and right
- make queue
- check empty
- dequeue front
- output front value
- for child in front.children breadth.enqueue(child)

- draw it out
- accomplish fizz buzz on whiteboard
- no external code required

- how do you clone a tree?
- cloned tree should be similar
- with fizz buzz, the values should be transformed

```{python}
import random

def encrypt(plain, shift):
  encrypted_test = ""

  for char in plain:
      num = int(char)
      shifted_num = (num + shift) % 10
      encrypted_text += str(shifted_num)

  return encrypted_text

def decrypt(encoded, key):
  return encrypt(encoded, -key)

if __name__ = "__main__":
  pins = [
    "1234",
    "9876",
    "0000",
    "9999",
  ]

  for pin in pins:
    key = random.randint(1, 9)
    print("plain pin", pin)
    encrypted_pin = encrypt(pin, key)
    print("encrypted_pin", encrypted pin)
    decrypted_pin = decrypt(encrypted_pin, key)
    print("decrypted_pin", decrypted_pin)
```

```{python}
import re
from corpus_loader import word_list, name_list

candidates = [
  "a dark and storm night"
  "fhue oi3 hfurei"
  "words words words"
]

def count_words(text):

    candidate_words = text.split()

    word_count = 0

    for candidate in candidate_words:
      word = re.sub(r'[^A-Za-z]+','', candidate)
      if word.lower() in word_list or word in name_list:

        word_count += 1

      else:
        pass
        # print('not english word or name', word)

    return word_count

  for phrase in candidates:

      word_count = count+Words(phrase)
      percentage = int(word_count / len(phrase.split()) * 100)
      if percentage > 50:
        print(phrase, percentage)
```

- is alpha for allowing non-alpha characters but ignoring them 
- built in method that will give numeric representation of that character
- 
