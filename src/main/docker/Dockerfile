#
# The app runs on port 8080 unless configured
# otherwise.
#
# The app can be enabled to pull its
# configuration from a Spring Cloud Config-Server.
#
FROM openjdk:8-jdk

MAINTAINER Smarter Balanced "opentestsystem.org"

VOLUME ["/tmp"]

COPY ap-irs.jar /

#RUN apk add --no-cache font-bakoma-ttf

#RUN apk add --no-cache --repository https://nl.alpinelinux.org/alpine/edge/testing font-bakoma-ttf

#RUN apk add --no-cache fonts-arphic-bkai00mp

#RUN apk --no-cache add curl

ENTRYPOINT ["/usr/bin/java"]

CMD ["-jar", "/ap-irs.jar"]
