# Class 17 

- Practice white board

find age range in tree

- when a tree gets past in you don't do self
- self is the current instance you are working in
- always ask if something is empty
- walk usually takes in the root
- if the root is none then don't do anything
- no change return back whatever came in
- move towards using peer functions
  - relies on input
  - responsible for output
- functional programming should be distributed across machines
- not a rule! push yourself to go there
- root points to a node or an oldest
- if there is no root than the youngest and oldests havent changed
- if root value (person object) is less than the youngest youngest becomes root value age
- else if person object is greater than the oldest, than the oldest becomes the root value
- then recurse
- walk(walk to the left, look at the youngest, look at the oldest)

Code Challenge 17

- Breadth first traversal
- first level is root
- uses a queue
- start at the root and enqueue
- entire node that has the value of A is at the front of the queue
- enqueue then dequeue the same node
- at the point of deuquee, enqueue its children 

- scraper.py
- http client to get http request
- pip install requests
- import requests
- freeze to requirements
- pip install beautiful soup
- from bs4 import Beuaitful Soup
- wants to know what the string to be parsed it 
- what kind of parsing do you want to be done
- soup.find(class_) is how to acess css in beautoful soup
- soup.find(class_="course=details")
- print(results.prettify())
- for title in titles:
    print(title.text)

    anchors = results("a")

    links - [anchor["href"] for anchor in anchors]

- use base path and append relative path 
- link soup
- another beautiful soup instance

- article - link_soup("article)[1]

- list_items = atricle.select("ul li ul li")

print(titles[1].text)
for li in list_items:
print(li.text)

