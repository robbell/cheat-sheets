# Docker

Connect a shell to a running *container*:

``` lang-sh
docker container exec --it [container] /bin/sh
```

Explore a docker *image*:

``` lang-sh
docker run --rm -it --entrypoint=/bin/sh [image]
```

_You can use the above to connect to intermediate stages of a docker build to explore the filesystem._

View real-time logging for a container:

``` lang-sh
docker logs -f [container]
```
