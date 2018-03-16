[hub]: https://hub.docker.com/r/spritsail/docker-build

# [spritsail/docker-build][hub]
[![](https://images.microbadger.com/badges/image/spritsail/docker-build.svg)](https://microbadger.com/images/spritsail/docker-build) [![](https://images.microbadger.com/badges/version/spritsail/docker-build.svg)][hub] [![Docker Stars](https://img.shields.io/docker/stars/spritsail/docker-build.svg)][hub] [![Docker Pulls](https://img.shields.io/docker/pulls/spritsail/docker-build.svg)][hub] [![Build Status](https://drone.spritsail.io/api/badges/spritsail/drone-docker-build/status.svg)](https://drone.spritsail.io/spritsail/docker-build)

## Supported tags and respective `Dockerfile` links

`latest` - [(Dockerfile)](https://github.com/spritsail/drone-docker-build/blob/master/Dockerfile)

## Configuration

```yaml
pipeline:
  build:
    image: spritsail/docker-build
    volumes: [ '/var/run/docker.sock:/var/run/docker.sock' ]
    repo: spritsail/docker-build
    dockerfile: Dockerfile-other
    directory: /tmp/workdir
    build_args:
      - BUILD_ARG=value
```
