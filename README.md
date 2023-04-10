# Cinema API
API service for cinema management written on DRF

## Install PostgresSQL and create db

- git clone https://github.com/SafonovVladimir/Cinema-API.git
- cd cinema-API
- python -m venv venv 
- source venv/bin/activate
- pip install -r requirements.txt

### Setup db
- set DB_HOST=your_db_hostname
- set DB_NAME=your_db_name
- set DB_USER=your_db_username
- set DB_PASSWORD=your_db_user_password
- set SECRET_KEY=your_secret_key

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