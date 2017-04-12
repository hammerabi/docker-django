This is a one-stop-shop for Django/Docker/DRF

You could use some REST.

# Requirements:


### Docker (https://www.docker.com/products/overview)

### Docker-compose (https://github.com/docker/compose)

### Docker-machine (https://github.com/docker/machine)

### VirtualBox (https://www.virtualbox.org/)

### pip



# Getting started:

First, create a virtual machine to run as a local Docker host ;)

`docker-machine create --driver virtualbox <your-container-name-here>`

Once that is up an running, change into this directory and run the following to build the project:

```
docker-compose pull

docker-compose build

docker-compose up
```



That's it!

To access `./manage.py`, from the project root, run `docker-compose run web bash`

--------------------------------------------------------------------------------

To make Database migrations:

```
docker-compose run web bash
#From this shell go:

./manage.py makemigrations

./manage.py migrate

```

--------------------------------------------------------------------------------

# Stack:

#### Python 2.7.9

#### Django 1.10

#### postgres:latest
