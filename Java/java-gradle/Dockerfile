FROM gradle:latest as builder
COPY . .
RUN gradle clean build
RUN pwd
RUN ls

FROM openjdk:8-jre-alpine
COPY --from=builder /home/gradle/build/libs/java-gradle-1.0-SNAPSHOT.jar /java-gradle-1.0-SNAPSHOT.jar
CMD [ "java", "-jar", "/java-gradle-1.0-SNAPSHOT.jar" ]