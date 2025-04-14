FROM maven:3.9.6-eclipse-temurin-17-alpine

USER root

# Install Docker CLI and Git
RUN apk add --no-cache docker-cli git

# Optional: Confirm tools are installed
RUN mvn -v && docker -v && git --version

CMD ["/bin/sh"]
