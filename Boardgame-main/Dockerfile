# Use OpenJDK 17 with Alpine base image
FROM openjdk:17-alpine

# Expose port 8080 for the Spring Boot application
EXPOSE 8080

# Set environment variable for application home directory
ENV APP_HOME /home/ec2-user

# Copy the SNAPSHOT jar from current directory to container
COPY *SNAPSHOT.jar $APP_HOME/app.jar

# Set the working directory to $APP_HOME
WORKDIR $APP_HOME

# Run the app when the container starts
CMD ["java", "-jar", "app.jar"]
