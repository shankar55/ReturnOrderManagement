FROM openjdk:8
ADD target/configserver.jar configserver.jar
EXPOSE 5555
ENTRYPOINT ["java","-jar","configserver.jar"]