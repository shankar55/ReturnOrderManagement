ReturnOrderManagement
--->we have automated the return order management through an web app, by classifying the process by repair or replacement.
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

--->BaseURL:http://localhost:5555

API-Gateway-Service
--->Spring Cloud Gateway aims to provide a simple, yet effective way to route to APIs and provide cross cutting concerns to them such as: security, monitoring/metrics, and resiliency.

--->BaseURL:http://localhost:1001

Authentication
--->https://medium.com/@mool.smreeti/microservices-with-spring-boot-authentication-with-jwt-and-spring-security-6e10155d9db0

--->BaseURL:http://localhost:2000

ReturnOrder Portal
--->This is the web layer where users can see the frontend of the webpage to enter the credentials in login page and redirect to home page where we can enter the return order packaging details.In this microservice, I have used html,css,Javascript.For different login user to login page we need to enter logout after BaseURL.

--->BaseURL:http://localhost:3000

<h3>Login page</h3>
<img src="images/login.PNG">
<hr>
<h3>Create Return Request Page</h3>
<img src="images/createreturnrequest">
<hr>
<h3>Confirm your order Request page</h3>
<img src="images/confirmrequestorder">
<hr>
<h3>Payment page</h3>
<img src="images/payment.PNG">
<hr>
<h3>paid page</h3>
<img src="images/paidpage.PNG">

Packaging-delivery
--->This is the backend Calculator to process the details of the user input fields and returns to payment page.

Payment
--->This microservice stores the payment details like cardnumber,cvv,username,payment in the credits table database. To test for RestAPI Endpoints we use postman.

--->Endpoint:http://localhost:8086/h2-console
<h4>h2-console in payment Microservice</h4>
<img src="images/h2-console.PNG">
<hr>
<h4>postman RestAPI Request</h4>
<img src="images/postman.PNG">


Component-Processing
--->This microservice invokes other microservices like portal, packaging-delivery,authentication,etc.


-------------------------------------------------------------------------------------------------------------------
How to set up this project locally in your machine?
-->we need to install a zip file from the repository.
-->we need to import all the files in eclipse or any IDE.
-->we need to add lombok.jar file externally in the properties.
-->we need to update the project forcefully in the maveen option.
-->we need to clean the project in the project option.

-------------------------------------------------------------------------------------------------------------------
Developed by: K Shankar