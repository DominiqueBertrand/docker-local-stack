# MockServer with Docker Compose

Whenever we are developing microservices, at some point we are going to come across some external dependency, and that can be a big headache.

To help with this issue, using a mock service for development. In addition to helping a lot when coding, it can also be very useful for testing, for example. [Here](https://www.mock-server.com/#why-use-mockserver) are some more benefits to use.

MockServer is very customizable, has many features, is very easy to configure, has a very nice debug UI and [the documentation is very complete](https://www.mock-server.com/mock_server/getting_started.html).

![MockServer](mockserver.avif)

His docker compose file [here](docker-compose.yml) , and inside the same folder there is a settings file, if you want to change these settings, just follow [this documentation](https://www.mock-server.com/mock_server/getting_started.html). 

To run:

```console
docker compose -f mock/docker-compose.yaml up -d

```

After uploading the containers, the UI will be available at: http://0.0.0.0:1080/mockserver/dashboard , and if you haven't changed the settings file, the test route will be: http://0.0.0.0:1080/hello