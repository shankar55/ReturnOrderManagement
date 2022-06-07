ReturnOrderManagement
-------------------------------------------------------------------------------------------------------------
Microservice Architecture
--->Microservices are a modern approach to software whereby application code is delivered in small,manageable pieces, independent of others.
-------------------------------------------------------------------------------------------------------------
System Architecture Diagram
<img src="images/ArchitectureDiag.PNG">
-------------------------------------------------------------------------------------------------------------
Eureka-Server
--->Eureka Server(Service-Registry) is an application that holds the information about all client-service applications. Every Micro service will register into the Eureka server and Eureka server knows all the client applications running on each port and IP address. Eureka Server is also known as Discovery Server.
BaseURL:http://localhost:8761

Config-Server
--->Central configuration server provides configurations (properties) to each micro service connected. Spring Cloud Config Server can be used as a central cloud config server by integrating to several environments.
BaseURL:http://localhost:5555

API-Gateway-Service
--->Spring Cloud Gateway aims to provide a simple, yet effective way to route to APIs and provide cross cutting concerns to them such as: security, monitoring/metrics, and resiliency.
BaseURL:http://localhost:1001

Authentication
--->https://medium.com/@mool.smreeti/microservices-with-spring-boot-authentication-with-jwt-and-spring-security-6e10155d9db0
BaseURL:http://localhost:2000

ReturnOrder Portal
--->This is the web layer where users can see the frontend of the webpage to enter the credentials in login page and redirect to home page where we can enter the return order packaging details.









