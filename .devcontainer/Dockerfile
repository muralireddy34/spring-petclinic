# FROM eclipse-temurin:17-jre-jammy
# WORKDIR /app
# COPY target/*.jar app.jar

# EXPOSE 8080
# ENTRYPOINT ["java", "-jar", "app.jar"]

FROM eclipse-temurin:17-jre-jammy
WORKDIR /app

# Print the current working directory in Docker build output
RUN echo "Current directory inside container:" && pwd
RUN echo "Listing files in working directory:" && ls -la

# Then copy the JAR
COPY target/*.jar app.jar

EXPOSE 8080
ENTRYPOINT ["java", "-jar", "app.jar"]
