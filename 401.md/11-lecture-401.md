# Class 11

- we will not have a full course on data science

code challenge

- implement a queue using two stacks
- queue is an idea 
  - enqueue dequeue, peek, empty
  - doing queues on array
  - all queues are FIFO or LILO
- instantiate stack objects in your constructor
- Python a constructor is initilaizer \__init__
- use stack instances from friday because we want to use them
- output means return value
- things in a stack HAVE to go on the top
- we want to dequeue the first IN
- when you get to last node you return it
- checking to see thatt here is no top
- keeping inbox and outbox in good shape
- dequeue means get from the top of the outbox
- if there is tuff in inbox that needs to be brought over from outbox do it
- there should enver be stuff in both stacks
- pop out of outbox and push into inbox

```{python}

class TwoStackQueue():
  def __init__(self):
    self.inbox = Stack()
    self.outbox = Stack()

  def enqueue(self, value):
    pass
    # push value ontop inbox

  def dequeue(self)
  # pop from outbox
  # do slinky as needed

q = TwoStackQueue()
print(q.inbox)
```

Lab 11

- render chess boards
- based on coordinates, figure out if queens are under attack
  - same row
  - same column
  - diagonal

- class should have a grid attribute
- grid means matrix
- RGB format

- make account with Kaggle
- chessboard
- share with public
- notebooks aren't always linear
- np stands for np 
- np arrays have to have the same data type
- matrices don't have to be square

```{python}

np.ones((8,8)) #is a 2d array

tensor = np.full((2, 4, 3), .5) #rows, columns, channels

# this will make 2 rows, of four columns where each thing is a value of .5
pixels = np.random.rand(4, 5, 3)

red = (1., 0., 0.) # red needs to be a tuple of intergers, so add decimals!
pixels = np.full((8, 8, 3), red)
plt.imshow(pixels)

green = (.1, .9, .05)
pixels = np.full((8, 8, 3), green)
plt.imshow(pixels)


orange = (1., .65, 0.)
checkered = np.full((4, 4, 3), orange)

// clunky way
checkered[0, 0] = green
checkered[0,2] = green
checked[1, 1] = green
checkered[1, 3] = green
checker3ed[2, 0] = green

plt.imshow(checkered)


// loopy way

checkered = np.full((4, 4, 3), orange)


for row_index, row_data in enumerate(checkered):
  for col_index, col_data in enumerate(row_data):
      if row_index % 2 == 0 and col_index % 2 != 0:
        checkered[row_index, col_index] = green
      if row_index % 2 != 0 and col_index % 2 == 0:
        checkered[row_index, col_index] = green
        if np.array_equal(checkered[row, col], purple):


plt.imshow(checkered)


// not loopy way

checked[::2, 1::2] = green
starting at index 0 go to the end every other row bill be hit
starting at 1 until the end, every other column
checkered[1::2, ::2] = green
starting at row 1, go until end every other row


// enumerate gives access to the index and the item


yellow = (.9, .9, .2)

checkered[2,3] = yellow
plt.imshow(checkered)
```

- notice loops and see if there is a way you can do it not in a loop


