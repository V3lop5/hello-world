FROM maven:latest as builder
COPY . .
RUN mvn clean compile assembly:single
RUN pwd
RUN ls

FROM openjdk:8-jre-alpine
COPY --from=builder /target/java-maven-1.0-SNAPSHOT-jar-with-dependencies.jar /java-maven-1.0-SNAPSHOT-jar-with-dependencies.jar
CMD [ "java", "-jar", "/java-maven-1.0-SNAPSHOT-jar-with-dependencies.jar" ]