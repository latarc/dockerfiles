FROM python:3-alpine

RUN apk add gcc musl-dev 
RUN python3 -m pip install ryu

CMD ryu-manager --observe-links ryu.app.rest_topology ryu.app.ofctl_rest
