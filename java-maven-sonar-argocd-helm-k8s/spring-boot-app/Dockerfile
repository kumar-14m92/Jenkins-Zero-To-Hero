FROM maven:3.9.6-eclipse-temurin-17-alpine

USER root

# Install docker CLI
RUN apk add --no-cache docker-cli

# Verify tools
RUN mvn -v && docker -v

CMD ["/bin/sh"]
