#
# Build stage
#
FROM gradle:7.2.0-jdk17 AS build
COPY . /app
RUN /app/gradlew init
RUN /app/gradlew build
EXPOSE 8080
ENTRYPOINT ["java","-jar","/app/build/libs/etronSystem-0.0.1-SNAPSHOT.jar"]
