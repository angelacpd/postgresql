# PostgreSQL
Learning how to integrate a PostgreSQL database to a Django project with Docker.

Based on Chapter 2 of book **Django for Professionals**:
https://wsvincent.com/books/

## Container

Build docker image
> docker build .

Start container (detached)
> docker-compose up -d

Stop container
> docker-compose down

Apply migrations
> docker-compose exec web python manage.py migrate

Create Django super user
> docker-compose exec web python manage.py createsuperuser