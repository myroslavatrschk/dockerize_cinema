# Cinema API

APi for cinema management written in Python using Django and Django Rest Framework.

## Installation via GitHub

Install PostgreSQL and create db

```
https://github.com/myroslavatrschk/dockerize_cinema
cd DRF-cinema-API
python -m venv venv
source venv/bin/activate (on MacOS/Linux)
venv\Scripts\activate (on Windows)
pip install -r requirements.txt
export DB_HOST=<your db hostname>
export DB_NAME=<your db name>
export DB_USER=<your db user>
export DB_PASSWORD=<your db password>
export SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver
```

## Run with Docker

Docker should be installed on your machine.

```
docker-compose build
docker-compose up
```

## To get access to work with api do next steps

```
create user via /api/user/register/
get access token via /api/user/token/
```

## Features

* JWT authenticated
* Admin panel localhost/admin/
* Documentation is located at localhost/api/doc/swagger/
* Managing orders and tickets
* Creating movies with genres, actors
* Creating cinema halls
* Adding movie sessions
* Filtering movies and movie sessions
