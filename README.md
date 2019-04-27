# django-postgres-docker

## Build the three containers
- postgres
- python 3
- django

## Images are automatically fetched, if necessary, from docker hub
docker-compose build

## Start a new web container to run migrations
Use --rm to remove the container when the command completes
docker-compose run --rm web python manage.py migrate

## Run everything in the background with -d
docker-compose up -d
