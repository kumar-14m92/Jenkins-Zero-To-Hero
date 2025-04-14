# Use a lightweight base image with Java 11 runtime
FROM adoptopenjdk/openjdk11:alpine-jre

# Pass the built JAR path as a build-time argument
ARG artifact=target/spring-boot-web.jar

# Set working directory inside the container
WORKDIR /opt/app

# Copy the JAR file into the container
COPY ${artifact} app.jar

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
