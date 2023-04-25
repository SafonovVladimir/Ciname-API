# Cinema API
API service for cinema management written on DRF

### Install PostgresSQL, create and setup db

- git clone https://github.com/SafonovVladimir/Cinema-API.git
- cd cinema-API
- python -m venv venv 

#### Linux/macOS:
- source venv/bin/activate
- pip install -r requirements.txt
- export DB_HOST=<your db hostname>
- export DB_NAME=<your db name>
- export DB_USER=<your db user>
- export DB_PASSWORD=<your db password>
- export DB_SECRET_KEY=<your secret key>
#### Windows: 
- venv\Scripts\activate
- pip install -r requirements.txt
- set DB_HOST=<your db hostname>
- set DB_NAME=<your db name>
- set DB_USER=<your db user>
- set DB_PASSWORD=<your db password>
- set DB_SECRET_KEY=<your secret key>

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
