FROM openjdk:8
ADD target/payment.jar payment.jar
EXPOSE 8086
ENTRYPOINT ["java","-jar","payment.jar"]