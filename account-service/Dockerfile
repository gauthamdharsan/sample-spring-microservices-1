FROM openjdk:8-jdk-alpine
RUN apk add maven
RUN mvn clean install .
ADD target/account-service.jar account-service.jar
EXPOSE 2222
ENTRYPOINT ["java", "-jar", "/account-service.jar"]
