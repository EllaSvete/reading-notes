# class 33

- relation error often means you need to migrate

- in dockercompse-yml

- volumes:
  - postgres_data: /var/lib/postgresql/data/


- outside of services:
  - volumes: 
    - postgres_data:

- docker volume command

- docker volume prune:
  - removes all local volumes not used by at least one ocntainer
  - gets rid of stuff that isnt being used 

- docker compose down
  - -v
- docker compose run web bash
- migrate
- createsuper user

- inside of your container:
- pip install djangorestframework-simplejwt
- docker compose run web bash

- cat requirements.txt
- pip3 freeze > requirements.txt
- exit docker terminal
- docker compose up
- go back into docker terminal and migrate and createsuperuser


- in urls.py from rest_framework_simplejwt import views aas jwt_views

- path("api/token/" jwt_views.TokenObtainPairView(), name="token_obtain_pair")

- go to api/token
- change in setting and add to requirements. txt!

- in lab list out for the grader how to test it
- explain where to get access token and do a get things

- Within the run web bash, do the pip install, the pip freeze in one session. Then do compose up --build. That should fix it.

- Gunicorn

- docker compse run web bash

- pip install gunicorn

- pip freeze > requirements.txt

- cat requirements.txt

- made a change so BUILD

- docker compose up --build

- in docker-compose
  - change command to gunicorn project_name

- make sure volumes match

- after rebuild you can do a restart

- docker compose down to run command again

- pip install whitenoise
- pip freeze requirements.txt

- middleware
  - add whitenoise.middleware.WhiteNoiseMiddleware

- static_root = base_dir / staticfiles

- docker compose up

- python manage.py collectstatic


- Code Challenge
  - all key value pairs on the left
  - any that match that are on the right

  - combine key and corressponding values in a left join flow
  - every nested array with have 3 items
  
