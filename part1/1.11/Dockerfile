FROM openjdk:8-jdk
EXPOSE 8080
COPY . /usr/src/app
WORKDIR /usr/src/app/spring-example-project
RUN ./mvnw package
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]
