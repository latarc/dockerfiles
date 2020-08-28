# OpenDaylight docker image

This is a docker image for the [OpenDaylight SDN Controller](https://www.opendaylight.org/).

## Commands

- Docker pull:
`docker pull latarc/opendaylight`

- Docker run:
`docker run -it --rm latarc/opendaylight`

## Default CMD

By default, the command executed after the `docker run` is `./bin/karaf`, which runs the ODL controller.

## Dockerfile

The Dockerfile for the latest version of this image is available on the [LaTARC Research Lab's Dockerfiles repository](https://github.com/latarc/dockerfiles).
