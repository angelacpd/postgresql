# PostgreSQL
Learning how to integrate a PostgreSQL database to a Django project with Docker.

Based on Chapter 2 of book **Django for Professionals**:
https://wsvincent.com/books/

## Commands to run this project

Build docker image
> docker build .

Start container (detached)
> docker-compose up -d

Apply migrations
> docker-compose exec web python manage.py migrate

Create Django superuser
> docker-compose exec web python manage.py createsuperuser

Log in Django admin with the superuser credentials

http://localhost:8000/admin/

Stop container
> docker-compose down