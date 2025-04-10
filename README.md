# Microservices Architecture with API Gateway
### This project demonstrates a simple microservices architecture with an API Gateway that routes requests to multiple services.
Services and Endpoints

User Service - Runs on port 8081 and can be accessed via http://localhost:8080/user/message

Admin Service - Runs on port 8082 and can be accessed via http://localhost:8080/admin/message

Welcome Service - Runs on port 8083 and can be accessed via http://localhost:8080/welcome/message

Eureka Server - Runs on port 8761 and can be accessed via http://localhost:8761

API Gateway - Runs on port 8080 and routes requests to the services

### Setup and Running Instructions
Prerequisites
- Java 17+
- Spring Boot
- Maven
- Eureka Server

### Running the Services
1. Start Eureka Server
- cd eureka-server
- mvn spring-boot:run

1. Start API Gateway
- cd eureka-server
- mvn spring-boot:run

2. Start Eureka Server
- cd api-gateway
- mvn spring-boot:run

3. Start User Service
- cd user-server
- mvn spring-boot:run

4. Start Admin Server
- cd admin-server
- mvn spring-boot:run

5. Start Welcome Server
- cd admin-server
- mvn spring-boot:run

### Accessing Services via Gateway

Once all services are up and running, you can access them through the gateway at port 8080:

User Service: http://localhost:8080/user/message

Admin Service: http://localhost:8080/admin/message

Welcome Service: http://localhost:8080/welcome/message

### Postman Collection

A Postman collection is attached to this project for making requests to the microservices via the API Gateway. You can import the collection into Postman to test the endpoints easily.

### Eureka Server

Eureka Server can be accessed at:
http://localhost:8761

### Conclusion

This project provides a basic implementation of a microservices architecture using Spring Cloud Gateway and Eureka for service discovery.
