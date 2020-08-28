FROM alpine

RUN apk update
RUN apk add --no-cache wget tar libstdc++ openjdk11
RUN wget https://nexus.opendaylight.org/content/repositories/opendaylight.release/org/opendaylight/integration/opendaylight/0.12.2/opendaylight-0.12.2.tar.gz
RUN tar -C /opt -xzf opendaylight-0.12.2.tar.gz
RUN rm opendaylight-0.12.2.tar.gz
WORKDIR /opt/opendaylight-0.12.2

# Install openflowplugin features then quit
# (there must be a better way to accomplish this)
RUN (echo -en "feature:install features-openflowplugin\nlogout\n") | ./bin/karaf
CMD ./bin/karaf