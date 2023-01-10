# dockerize-cinema

# Cinema API

Api service for cinema management written on DRF

# Installing using GitHub

Install PostgresSQL and create db

```shell
git clone https://github.com/Pavilion4ik/dockerize-cinema.git
cd dockerize-cinema
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
set DB_HOST=localhost
set DB_NAME=dockercinema
set DB_USER=dockercinema
set DB_PASSWORD=dockercinema
set SECRET_KEY=django-insecure-6vubhk2$++agnctay_4pxy_8cq)mosmn(*-#2b^v4cgsh-^!i3
python manage.py migrate
python manage.py runserver
```

# Run with docker
Docker should be installed

```shell
docker-compose build
docker-compose up
```


# Getting access
* create user via /api/user/register
* get access token via /api/user/token


# Features
* JWT authenticated
* Admin panel /admin/
* Documentation is located at api/doc/swagger/
* Managing order and tickets
* Creating movies with genres, actors
* Creating cinema halls
* Adding movie sessions
* Filtering movies and movies sections