FROM gradle:latest as builder
COPY . .
RUN gradle clean build
RUN pwd
RUN ls

FROM openjdk:8-jre-alpine
COPY --from=builder /home/gradle/build/libs/kotlin-gradle-kts-1.0-SNAPSHOT.jar /kotlin-gradle-kts-1.0-SNAPSHOT.jar
CMD [ "java", "-jar", "/kotlin-gradle-kts-1.0-SNAPSHOT.jar" ]