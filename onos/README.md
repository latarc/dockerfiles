# ONOS docker image

This is a docker image for the [ONOS SDN Controller](https://www.opennetworking.org/onos/).

## Commands

- Docker pull:
`docker pull latarc/onos`

- Docker run:
`docker run -it --rm latarc/onos`

## Default CMD

By default, the command executed after the `docker run` is `bash /opt/onos/bin/onos-service start`, which runs the ONOS controller. It is essential to run the service script with `bash` or other compatible shell (running with `/bin/sh` gives an error).

## Dockerfile

The Dockerfile for the latest version of this image is available on the [LaTARC Research Lab's Dockerfiles repository](https://github.com/latarc/dockerfiles).
