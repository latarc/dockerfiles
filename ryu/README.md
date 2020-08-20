# Ryu docker image

This is a docker image for the [Ryu SDN Framework](https://github.com/faucetsdn/ryu).

## Commands

  - Docker pull: 
`docker pull iwaseyusuke/mininet`

  - Docker run:
`docker run -it --rm latarc/ryu`

## Default CMD

By default, the command executed after the `docker run` is:

`ryu-manager --observe-links ryu.app.rest_topology ryu.app.ofctl_rest`

This command starts Ryu with both the `rest_topology` and `ofctl_rest` applications, which listen on TCP port `8080`.

## Dockerfile

The Dockerfile for the latest version of this image is available on the [LaTARC Research Lab's Dockerfiles repository](https://github.com/latarc/dockerfiles).
