## 1. Which base image do you want to use?
FROM maven:3.8.7-openjdk-18-slim

## 2. Set the working directory.
WORKDIR /app/

## 3. Copy the application's project files into the working directory.
COPY /springboot-demo/ .

## 4. Document and inform the developer that the application will use the container port: 8080.
EXPOSE 8080

## 5. Define the command to run when the container starts.
RUN ["mvn", "package"]
CMD ["java", "-jar", "target/demo-0.0.1-SNAPSHOT.jar"]