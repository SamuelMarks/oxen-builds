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
E.g., https://github.com/Oxen-AI/Oxen/releases/download/v0.18.15/oxen-ubuntu-latest.deb

Extract out `oxen-server`. Now you can run:
```sh
docker build -f Dockerfile.distroless -t samuelmarks/oxen-builds:distroless_cc-debian12_oxen_server_v0.18.15 .
```

Then to `run` you simply:
```sh
docker run samuelmarks/oxen-builds:distroless_cc-debian12_oxen_server_v0.18.15
```

And to `push` up to hub.docker.com run:
```sh
docker push samuelmarks/oxen-builds:distroless_cc-debian12_oxen_server_v0.18.15
```

<small>
## License

Licensed under either of

- Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or <https://www.apache.org/licenses/LICENSE-2.0>)
- MIT license ([LICENSE-MIT](LICENSE-MIT) or <https://opensource.org/licenses/MIT>)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.
</small>
