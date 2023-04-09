# Mongo Stack with Docker Compose

A simple Mongo Stack in docker using docker-compose.

Designed to be quick and simple to get a local or test environment up and running. Needless to say... 

**It's important that you have at least a base on [Docker](https://www.docker.com/) and [Docker Compose](https://docs.docker.com/compose/) and of course, have it [installed](https://www.docker.com/products/docker-desktop) on your machine.**

**DON'T USE THIS IN PRODUCTION!**

## How to run mongodb and mongo express with docker

Before starting the tools, we will create a network for our containers, as we will have several different files for our stacks, so you can more easily choose which one to use and when.

```console
docker network create global-default
```

For Mongo, it was very simple to build something that already solves our need locally. We also put mongo-express on configurationcompose help with debugging.

To run:

```console
docker compose up --force-recreate -d 
```

mongo-express will be available at http://0.0.0.0:8081/ .