# fastapi-tdd-docker

fastapi-tdd-docker course from testdriven.io

# Test-Driven Development with FastAPI and Docker

![Continuous Integration and Delivery](https://github.com/jcgentr/fastapi-tdd-docker/workflows/Continuous%20Integration%20and%20Delivery/badge.svg?branch=main)

# docker-compose start app

`docker-compose up -d --build`

# docker-compose stop app

`docker-compose down -v`

# docker-compose follow logs

`docker-compose logs --follow --timestamps web `

# run test with coverage

`docker-compose exec web python -m pytest --cov="."`

## and output html

`docker-compose exec web python -m pytest --cov="." --cov-report html`

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
