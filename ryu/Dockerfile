FROM python:3-alpine

RUN apk add gcc g++ musl-dev 
RUN python3 -m pip install ryu eventlet==0.30.2

ENTRYPOINT ["ryu-manager", "--default-log-level=30", "--observe-links", "ryu.app.rest_topology", "ryu.app.ofctl_rest"]
