# ONOS docker image

This is a docker image for the [ONOS SDN Controller](https://www.opennetworking.org/onos/).
When running ONOS, the `org.onosproject.openflow` app is automatically activated. The default user and password of the ONOS GUI,
and of the openflow app's REST API is `onos` and `rocks`, respectively.
In addition, the ONOS CLI is accessible via `ssh` on port `8180`, with the user `karaf` and password `karaf` as well.

## Commands

- Docker pull:
`docker pull latarc/onos`

- Docker run:
`docker run -it --rm latarc/onos`

## Default CMD

By default, the command executed after the `docker run` is `bash /opt/onos/bin/onos-service start`, which runs the ONOS controller. It is essential to run the service script with `bash` or other compatible shell (running with `/bin/sh` gives an error).

## Dockerfile

The Dockerfile for the latest version of this image is available on the [LaTARC Research Lab's Dockerfiles repository](https://github.com/latarc/dockerfiles).
