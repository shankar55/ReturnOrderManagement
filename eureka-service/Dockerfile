FROM openjdk:8
ADD target/eureka-service.jar eureka-service.jar
EXPOSE 8761
ENTRYPOINT ["java","-jar","eureka-service.jar"]