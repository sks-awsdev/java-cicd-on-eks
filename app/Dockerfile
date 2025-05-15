# Use an OpenJDK runtime base image
FROM openjdk:17-jdk-slim

# Set working directory inside container
WORKDIR /app

# Copy the built JAR from Jenkins build context
COPY target/devops-app-1.0-SNAPSHOT.jar app.jar

# Expose port (optional, useful for Spring Boot etc.)
EXPOSE 8080

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
