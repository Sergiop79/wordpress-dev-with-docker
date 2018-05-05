# WordPress development with Docker

## Requirements

+ [Docker](https://www.docker.com/community-edition)
+ [Docker-compose](https://docs.docker.com/compose/)

To run for first time this environment:

```
$ docker-compose up
``` 

To start the containers

```
$ docker-compose start
``` 

To stop the containers

```
$ docker-compose stop

``` 
To remove and stop the containers

```
$ docker-compose down
``` 

The WordPress site is in [localhost](http://localhost), for the first time when the containers are created, starts the WordPress installation.

## WordPress files

The WordPress files will save in the `wordpress-data` folder.

## WordPress mysql database

The database will be stored in a named docker volume for example `your-project-folder_db_data`.

You can see this running:

```
$ docker volume ls
```

## PhpMyAdmin

You can manage the database with PhpMyAdmin on [localhost:8080](http://localhost:8080).

The user will be `MYSQL_USER` variable and the password `MYSQL_PASSWORD` in `docker-compose.yml` file.