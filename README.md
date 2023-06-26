# Spring Boot REST API microservice

A spring boot REST API microservice with MySQL DB backend. It has been dockerized for easier build and local deployment.

## Build Docker Container

The following command will build the docker container with maven and Java 17.

``` bash
docker-compose build
```

## Running the service

The following command will run the spring boot service with MySQL DB with nginx as reverse proxy.

``` bash
docker-compose up
```

Three containers will start and port `81` will be exposed.

## Sample Run

``` bash
$ curl localhost:81
I have been seen ip 10.247.7.3 1 times.
$ curl localhost:81
I have been seen ip 10.247.7.3 2 times.
$ curl localhost:81
I have been seen ip 10.247.7.3 3 times.
```
