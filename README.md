# fe-dev-docker

> Personal frontend develop environment.

### Usage

```bash
# install docker
$ brew install docker

# download image
$ docker pull ifyour/fe-dev-docker

# create container
$ docker run \
         -itd \
         -p <work-port>:8080 \
         -v <work-path>:/workspace \
         --name my-frontend-dev-env \
         --restart ifyour/fe-dev-docker
# eg:
$ docker run \
         -itd \
         -p 80:8080 \
         -v ~/Documents/Projects:/workspace \
         --name my-frontend-dev-env \
         --restart ifyour/fe-dev-docker

# operate container
$ docker exec -it my-frontend-dev-env zsh

# delete container
$ docker rm -f my-frontend-dev-env
```

### Reference

- [Docker Hub](https://hub.docker.com/r/ifyour/fe-dev-docker)
- [Docker 5 分钟入门](https://github.com/ifyour/ifyour.github.io/issues/42)

### License

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
