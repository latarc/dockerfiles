FROM python:3.8-alpine

RUN apk update --no-cache
RUN apk upgrade --no-cache
RUN apk add --no-cache gcc g++ musl-dev 
RUN python3 -m pip install ryu networkx eventlet==0.30.2

ENTRYPOINT ["ryu-manager", "--default-log-level=30", "--observe-links", "ryu.app.rest_topology", "ryu.app.ofctl_rest"]
