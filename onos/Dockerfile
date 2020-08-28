FROM alpine

RUN apk update
RUN apk add --no-cache wget tar bash curl openjdk11
RUN wget https://repo1.maven.org/maven2/org/onosproject/onos-releases/2.4.0/onos-2.4.0.tar.gz
RUN tar -C /opt -xzf onos-2.4.0.tar.gz
RUN rm onos-2.4.0.tar.gz
RUN mv /opt/onos-2.4.0 /opt/onos
WORKDIR /opt/onos

CMD bash /opt/onos/bin/onos-service start