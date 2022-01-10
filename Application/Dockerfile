FROM mcr.microsoft.com/java/maven:8u192-zulu-debian9 AS build-env
WORKDIR /app
COPY . /app
# RUN mvn package

COPY /app/target/*.jar /app.jar
ENTRYPOINT ["java","-jar","/app.jar"]