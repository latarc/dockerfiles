FROM alpine

RUN apk update
RUN apk add --no-cache openjdk8 g++ make apache-ant maven python-dev git
RUN git clone git://github.com/floodlight/floodlight.git
WORKDIR /floodlight
RUN git submodule init
RUN git submodule update
RUN mvn clean install
RUN mkdir /var/lib/floodlight
RUN chmod 777 /var/lib/floodlight
RUN apk del git

# Floodlight config in file target/classes/floodlightdefault.properties

CMD java -jar target/floodlight.jar