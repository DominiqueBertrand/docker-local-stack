# Local development environment using docker

Creating a local development environment can seem like a challenge. Who never suffered ~ at least a little ~ to get the dependencies running on their machine to create a project?

We usually go through that almost every time. Before discovering Docker, this was much more difficult... Having to upload a database locally always caused some kind of headache, even more so when you needed to have a specific version due to an existing project that needed to be updated. maintenance.

The idea is to help you set up a local development environment quickly and easily using everything with Docker. Also, I'll show you some support tools that can help a lot when debugging some things.

It's important that you have at least a base on Docker and Docker Compose and of course, have it installed on your machine.

To make it easier, I suggest that you clone the project that I prepared for this article with all the files ready.


```console
git clone git@github.com:dominiquebertrand/docker-local-stack.git
```

Before starting the tools, we will create a network for our containers , as we will have several different files for our stacks, so you can more easily choose which one to use and when.

```console
docker network create global-default
```