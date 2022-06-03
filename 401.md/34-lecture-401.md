# Class 34 Lab

- make a copy of the template and clone down
- cat docker-compose.yml
- environment is the container
- in container
- python -c "import secrets; print(secrets.token_urlsafe())"
- make sure you have 0.0.0.0 in allowed_hodts in ENV
- test container and then getout of it
- change things to the app name you want
- check that it was changed in settings
- cnahged in snacks
- changed in urls
- changed in permissions?
- Make sure model is changed!
- app
- admin
- views
- serializers
- BEFORE MIGRATE
- change fields!!!!
- do a global search to ensure you didnt miss any
- switch to container
- migrate
- createsuperuser

- brew install httpie

- on app side goto databases
- env.str
- when you use django environ

- database name is hwat we get from the user and default data base in elephant
  - ncqnpslj
  - this goes in env for user and name
  - same for password
  - yU2amU23nZVUCkwRguI2xhGDCXE2FYUB
  - same for database host
    - heffalump.db.elephantsql.com
  - port 5432
    - this default port for postgres

- after env chnaged make sure you rebuild!

- docker compose run web bash
  - pip install psycopg2-binary
  - then freeze
  - docker compose build
  - migrate again in container
  - super user

- heroku apps:create unique_name
- heroku.yml
  - yet another markup language
  - check names

- in regular terminal
- heroku stack:set container
- this deploys in a docker container

- not tying heroku to github
- git add
- git commit 
- git push heroku main

- in heroku add the env variables 

- csrf stuff
