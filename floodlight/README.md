# Floodlight docker image

This is a docker image for the [Floodlight SDN Controller](https://floodlight.atlassian.net/wiki).

## Commands

- Docker pull:
`docker pull latarc/floodlight`

- Docker run:
`docker run -it --rm latarc/floodlight`

## Default CMD

By default, the command executed after the `docker run` is `java -jar target/floodlight.jar`, which runs the Floodlight controller.

## Dockerfile

The Dockerfile for the latest version of this image is available on the [LaTARC Research Lab's Dockerfiles repository](https://github.com/latarc/dockerfiles).
