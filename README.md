# Symfony 5 docker-compose template
Template to host Symfony 5 applications on docker with PHP and MySQL

## Installation
1. Clone repository
2. `docker-compose up -d`

## Run new symfony project
```
# CREATE NEW PROJECT INTO CONTAINER (because containing composer)
docker-compose exec php composer create-project symfony/website-skeleton .

# CHANGE PERMISSION TO EDIT FILES
sudo chown -R $(id -un):$(id -gn) www
```