# Use a basic OpenJDK image
FROM openjdk:17-jdk-slim

# Set the folder inside the container
WORKDIR /app

# Copy the JAR file (after building with Maven or Gradle)
COPY target/devops-app-1.0-SNAPSHOT.jar app.jar

# Expose port (your app usually runs on 8080)
EXPOSE 8080

# Run the JAR file
ENTRYPOINT ["java", "-jar", "app.jar"]
