FROM maven:3.9-eclipse-temurin-17
WORKDIR /app

COPY pom.xml .
RUN mvn dependency:resolve

COPY src src
RUN --mount=type=cache,target=/root/.m2 mvn package

EXPOSE 8080
ENTRYPOINT ["java", "-jar", "target/api.jar"]