# Containerisation for data science: part i

by Alecia Vogel at Cybera

## Introduction

* synchronising computing environments
	* automates this boring work
	* helps with reproducibility
	* docker is the only requirement
* virtual machines used to isolate each application in its own environment
	* almost always running Linux
* common use case is server side code

## Idea

* you need to tell the virtual machine which packages you need
* these instructions are written in a dockerfile
	* we will use docker-compose which is an easy version

## Getting started

* `docker-compose up`

## Ports

The `docker-compose.yml` file requires us to specify the appropriate ports.

Port notation: `abcd:wxyz` the latter is the one we link to.
(The former is the allocation on your computer.)
In other words: `wxyz` is the port it is listening on.
The port `abcd` is the port on our computer we are accessing from.
* so if they are different we must modify the link we use

* one can specify multiple ports

## Add your own files and directories

Need to mount the volume.
* simply add a `volume:` entry to the `docker-compose.yml`.
* need a string with a colon in
	* e.g. `./:/home/jovyan` the latter is where is gets mounted to and 
	the former is what we want to mount

## Environment variables

Simply add then to an `environment:` entry in the `docker-compose.yml`.

In this case we need to enable jupyter lab to be on.

## Build dependencies

Add a `depends_on:` entry to `docker-compose.yml`.

# Containerisation: part ii

Can use modules in the `docker-compose.yml` by using the `build:` tag.

The PHP host will be the name of the service in the docker compose that has the database.