# Class 3

## Code Challenge and Warm Up

- sort list in place means it doesn't want a new linked list
- got through the linked list and put in a new list then sort that list
- selection sort
- temp value to hold values and then shift over comparing values
- time in Big(O) in N
- space in Big(O)1 because constant

- linked list - usually mess with the pointers not the values!
- sometimes you have to mess with the values

- isntead of casting to bool check if its None

## Lab

- Only authenticated users can get access to API
- appropriate yser can update or delete (owner)
- add ability to log in and out
- docker compose up 
  - if never then built then it will build container
  - -- build: will trigger rebuild
  - don't run postgres directly on host machine
    - we will be doing it in a container
    - createsuperuser and migrate will need to happen inside container
    - not in host!

- docker compose run web bash
  - this will jump inside container
  - python -V to check its running in container
  - python manage.py showmigrations
  - only difference is we are inside the container
    - we do NOT need venv
    - python manage.py migrate
    - python manage.py createsuperuser
    - login button is connect to superuser

- admin panel to make a new user
- go to site url 
- new user can see the data and add a new "thing" but cannot edit existing things
- exit to get out of container

- docker compose down to remove container and network
- up, down, run are most common commands

- in rest framework 
  - default permission classes
  "rest_framework.persmissions.IsAuthenticated",
- not built in but you must make the change to IsAuthenticated

- Login is new
- allowed hosts you add '0.0.0.0'
- also allow localhost
- '123.0.0.1,'

- url patterns make some path that has restframework urls

- custom permissions in ways that go beyond the default

- make python file 
  - permissions.py

  - from rest framework import permissions

  - make a class

  - class IsOwnerOrReadOnly(permissions.BasePermission):
  
  - def has_object_permission(self, request, view, obj):

    - read only unless destructive action
    - only want things to change if it's the owner

    - if request.method in permissions.SAFE_METHODS:

      - gets should be safe and not make changes

      - return True

      - if obj.owner is None
        - deals with cases where you have resource but doesn't have an owner

        - return True

     - if obj.owner == request.user

- how do we get this class into use?
  - head over to views.py

  - permission_classes = (IsOwnerOrReadOnly,)
    - have comma to show its tuple

- create dockerfile 

-  psycopg2-binary

- 11:40pm in video

- containers are ephemeral 

- do not run postgress on machine!!
