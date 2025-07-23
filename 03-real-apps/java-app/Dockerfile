FROM amazoncorretto:11-alpine

WORKDIR /app

# Copy everything
COPY . .

# Build the application
RUN ./mvnw package -DskipTests

EXPOSE 4567

ENTRYPOINT ["java", "-jar", "target/java-app-demo-1.0.0.jar"]
