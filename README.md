Oxen builds
===========
[![Docker Image Version (tag)](https://img.shields.io/docker/v/samuelmarks/oxen-builds/distroless_cc-debian12_oxen_server_latest)](https://hub.docker.com/r/samuelmarks/oxen-builds/tags)
[![docker_build](https://github.com/SamuelMarks/oxen-builds/actions/workflows/docker_build.yml/badge.svg)](https://github.com/SamuelMarks/oxen-builds/actions/workflows/docker_build.yml)

Builds for https://github.com/Oxen-AI/Oxen

Experimenting with different build setups for easy distribution of `oxen` and `oxen-server`.

For Docker images, see: https://hub.docker.com/r/samuelmarks/oxen-builds

## Instructions

### Docker build

Download the .deb file:
E.g., https://github.com/Oxen-AI/Oxen/releases/download/v0.15.16/oxen-ubuntu-latest.deb

Extract out `oxen-server`. Now you can run:
```sh
docker build -f Dockerfile.distroless -t samuelmarks/oxen-builds:distroless_cc-debian12_oxen_server_v0.15.16 .
```

Then to `run` you simply:
```sh
docker run samuelmarks/oxen-builds:distroless_cc-debian12_oxen_server_v0.15.16
```

And to `push` up to hub.docker.com run:
```sh
docker push samuelmarks/oxen-builds:distroless_cc-debian12_oxen_server_v0.15.16
```
