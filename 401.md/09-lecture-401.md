# Class 9

- if you can stringify it in this order
- reverse
- compare in stringified form
 - reverse it
 - and unreversed and compare them

```{python}
def get_scorers(roll)
"""
turn (1, 2, 3, 1, 5)
into (1, 1, 5)

1, 2, 3, 1, 5, == 250 Original Score
2, 3, 1, 5 == 150 - first 1 counted toward scoring
1, 3, 1, 5 == 250 - second element did NOT contribute
"""

all_dice = list(roll)

# iterate through toll values
# removing one at a time to see if score effected
# add to scorers

scorers = []


def validate_keepers(roll, keepers):
counted_roll = COunter(roll)

counted_keepers = Counter(keepers)

for num in counted_keepers:
  if counted_keepers[num] > counted_roll[num]:
    return False

return True

```


- Palindrome

- take linked list and put inside and array
- memory O(N) because of the amount of steps 
- check the values of each i


def isPalindrome(self, head: ListNode) -> bool:
nums = []

- putting this inside of array

while head:

nums.append(head.val)
head = head.next

- update pointer

l, r = 0, len(nums) - 1
while l <= r:
pointers don't cross, but check if they have same chracter
if nums [l] != nums[r]:
if nums of left does not equal nums of right, NOT palidrome
return False

l += 1
r -= 1

return True

- Reverse Linked List

- use two pointers
- 

def reversedList(self, head)

define pointers
prev, current = None, head

while current is not NUll reverse the pointers
while current:
nxt = current.next is temproary variable
current.next = prev
prev = current
current = current.next


return previous

- time Big O of N memory big O of O1