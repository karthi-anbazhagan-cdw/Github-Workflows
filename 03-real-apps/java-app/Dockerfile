FROM amazoncorretto:11-alpine

RUN apk add --no-cache maven

WORKDIR /app

# Copy everything
COPY . .

# Build the application
RUN mvn package -DskipTests

EXPOSE 4567

ENTRYPOINT ["java", "-jar", "target/java-app-demo-1.0.0.jar"]
