# docker-frp
frp server Dockerfile.
## Note:
> this project need [frp](https://github.com/fatedier/frp.git), need move Dockerfile and config file to frp project directory build.

```bash

$ DOCKER_BUILDKIT=0 docker build -f Dockerfile-for-frps  -t frps:latest .
$ DOCKER_BUILDKIT=0 docker build -f Dockerfile-for-frpc  -t frpc:latest .
$ docker-compose -f docker-compose-frps up -d
$ docker-compose -f docker-compose-frpc up -d
$ docker-compose -f docker-compose-frps logs -f
$ docker-compose -f docker-compose-frpc logs -f
```
