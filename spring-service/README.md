# React Spring Fullstack Demo
This is the part of the service project which is built with Spring boot3.
This is quite simple demo just serve one api, However, still adhere to reasonable design patterns.

---
## Development environment
- JDK 17 +
- Maven 3.5 +
- IntelliJ IDEA
- Mysql 5.7 +

## Running the app

To run the app, follow these steps:

```
cd spring-service
mvn clean package
java -jar target/backend-0.0.1-SNAPSHOT.jar
```
when development this project make sure that `mvm package` will automatically package docker image and publish the image to you docker hub.
However, you can package docker image use `Dockerfile` by manual.

OR

You can use `docker-compose.yml` one key start all services, or follow below steps to start backend:
- step 1: install mysql and run `mydemo.sql` script to setup database.
- step 2: pull docker backend image `docker pull claydocker/spring-service:latest` and start it with default port `8080`.
- step 3: once finished those you can visit this api `http://you-ip/api/v1/food-trucks`

## Tech Stack
- Java
- Spring Boot
- JPA
- Jib
- Docker
- MySQL
- REST API


