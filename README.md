# fastapi-tdd-docker

fastapi-tdd-docker course from testdriven.io

# docker-compose start app

`docker-compose up -d --build`

# docker-compose stop app

`docker-compose down -v`

# docker-compose follow logs

`docker-compose logs --follow --timestamps web `

# run linting

`docker-compose exec web flake8 .`

# run formatting

`docker-compose exec web black .`

## check only

`docker-compose exec web black . --check`

# run import sorting

`docker-compose exec web isort .`

## check only

`docker-compose exec web isort . --check-only`
