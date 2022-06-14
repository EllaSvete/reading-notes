# class 39

## Linked List

- Traversing linked list
  - while loop until current is None

- make head point to the previous


## lab 39

- use data from remote api
- as long as youre on a different port it is different enough 
- even if API is deployed, as soon as you get another client there is the chance for API to not allow communication
- it will ask do we really want to allow this
- not requirement to be remote today

- there are some tweaks that will be made for version 3
- logged in and not logged in
- cookie stand admin logged in form 
- ability for frontend to sign in and sign out
- data should be posted to an API
- cookiestand table should render new row and appending state
- add delete icon to delete the stand, shouldnt require page refresh, and API should know about it
- continue to work in same repo
- front end will communicate with api you built
- OR there is a test api available
- is everything we need to do purely front end?
  - no! backend is responsible for that
  - need ability to log in
  - getting email back would be greay
  - token is only meant for email right now

from datetime import time delta

simple_jwt ={

  "access_toke_lifetime": timedelta(
    seconds=60*60
  ),
}

- add projects view
- 
