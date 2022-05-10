# Class 16

## Code REview

"Review:

- pre - Root is at the start of the list
  - Good if you're trying to rebuild the tree and wanted to add them
  - End up with an order thats not 100% correct but it's your best short
- post - root is at the end of the list
  - If you think about them as containing operations (maybe you have network operations) each thing has some sort of resources with it so we don't properly dispose of a root until the children are gone
  - no memory leaks or anything.
- in - root is IN the middle of the list
  - Really good in binary search traversal so it will maintain the order
  - will maintain the values of the nodes as ints

Find a max of a binary tree

- extending an implementation
  - going to be writing a method on the binary tree
- (not binary search tree) it'd be easy to find the max in the binary search tree, cause you'd just go to the right!
- But in a binary tree! that's more difficult cause there aren't rules of where things are placed
- no arguments
non-local approach (JB throwin it out there, so you can ask about it if you want to)
Pass everything in and return out only what's needed, no actual modifications (preferred approach, not a rule)

## Lab

- .vercel command line will be in gitignore
- gh browse
- api folder, api in the route name
- vercel cli
  - deploy command
  - vercel -h
  - vercel dev
  - y

- query parameters
  - key value pairs
  - aloha?name=Ben

  from http.server import BaseHttpRequestHandler
  from urllib import parse

class handler(BaseHttpRequestHandler)
  def do_GET(self):

    path = self.path
    url_components = parse.urlsplit(path)
    query_string_list = parse.parse_qsl(url_components.query)
    dic = dict(query_string_list)

    self.response(200)
    self.sned_header("Content-type", "text/plain")
    self.end_headers()

    name = dic.get("name")

    if name:
      message = f"Aloha {name}"
    else:
      message = "Aloha stranger"

    message = f"{name}"

    self.wfile.write(message.encode())
    return

- set up and activate venv
- pip install requests
- pip freeze > requirements.txt

import requests

class handler(BaseHttpRequestHandler)
  def do_GET(self):

    s = self.path
    path = self.path
    url_components = parse.urlsplit(path)
    query_string_list = parse.parse_qsl(url_components.query)
    dic = dict(query_string_list)

    if "word" in dic:
      url = "www..api.."
      full_url = url + dic["word"]
      response = requests.get(full_url)
      data = response.json()

      definitions = []
      for word_data in data:
          definition = word_data["meanings"][0]["defintions"][0]["deinftion"]
          definitions.append(definition)
      
      message = str(definitions)  

    else: 
      message = "give me a word"

    self.response(200)
    self.sned_header("Content-type", "text/plain")
    self.end_headers()

    self.wfile.write(message.encode())

     return

