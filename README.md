# Commands

`
docker-compose run --rm app sh -c "python manage.py test && flake8"
`

## Make Migrations

`
docker-compose run --rm app sh -c "python manage.py makemigrations"
`

## Migrate

`
docker-compose run --rm app sh -c "python manage.py migrate"
`
## Collect Static Files

`
docker-compose run --rm app sh -c "python manage.py collectstatic --noinput"
`
