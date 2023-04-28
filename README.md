# Cinema API
API service for cinema management written on DRF

### Install PostgresSQL, create and setup db

- git clone https://github.com/SafonovVladimir/Cinema-API.git
- cd cinema-API
- python -m venv venv 

#### Linux/macOS:
- source venv/bin/activate
- pip install -r requirements.txt
- export POSTGRES_HOST=<your db hostname>
- export POSTGRES_DB=<your db name>
- export POSTGRES_USER=<your db user>
- export POSTGRES_PASSWORD=<your db password>
- export SECRET_KEY=<your secret key>
#### Windows: 
- venv\Scripts\activate
- pip install -r requirements.txt
- set POSTGRES_HOST=<your db hostname>
- set POSTGRES_DB=<your db name>
- set POSTGRES_USER=<your db user>
- set POSTGRES_PASSWORD=<your db password>
- set SECRET_KEY=<your secret key>

### Run server
- python manage.py migrate
- python manage.py runserver

### Run with docker
Docker should be installed

- docker-compose build
- docker-compose up

### Getting access
- create user via /api/user/register/
- get access token via /api/user/token/

## Features
- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres and actors
- Creating Cinema halls
- Adding movies sessions
- Filtering movies and movie sessions

# Endpoints:
![](readme_screenshots/1.jpg)

![](readme_screenshots/2.jpg)

![](readme_screenshots/3.jpg)
* Filtering
![](readme_screenshots/4.jpg)
