# Java 21 runtime image (recommended)
FROM eclipse-temurin:21-jre

# Path of jar produced by Maven build
ARG JAR_FILE=target/spring-boot-web.jar

WORKDIR /opt/app

# Copy jar into image
COPY ${JAR_FILE} app.jar

# Optional: expose your app port (change if different)
EXPOSE 8080

# Run app
ENTRYPOINT ["java","-jar","app.jar"]
