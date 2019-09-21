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

RUN apt-get update

RUN apt-get -y install curl libunwind8 gettext apt-transport-https

RUN apt-get -y install jq

CMD ["java", "-jar", "/ap-irs.jar"]
