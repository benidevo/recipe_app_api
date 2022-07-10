# Recipe API

## Description

    The Recipe API is a RESTful API that allows you to create, update, and delete recipes.
    The API is based on the [Swagger](https://swagger.io/) specification.

## Technologies

The following technologies were used in this project:

- [Python](https://www.python.org/)
- [Django](https://www.djangoproject.com/)
- [Django REST Framework](https://www.django-rest-framework.org/)
- [PostgreSQL](https://www.postgresql.org/)
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/overview/)
- [AWS](https://aws.amazon.com/)

## Requirements

Before starting, you need to have [Python](https://www.python.org/) installed. Also ensure to create a .env file in the root directory of the project, and provide the environment variables in .env.example file.

## Commands

Kindly ensure that you are in the root directory before running the following commands.

### Build the project

`
docker-compose build
`

### Run the container

`
docker-compose up
`

### Stop the container

`
docker-compose down
`

### Run Tests

`
docker-compose run --rm app sh -c "python manage.py test && flake8"
`

### Make Migrations

`
docker-compose run --rm app sh -c "python manage.py makemigrations"
`

### Migrate

`
docker-compose run --rm app sh -c "python manage.py migrate"
`

### Collect Static Files

`
docker-compose run --rm app sh -c "python manage.py collectstatic --noinput"
`
