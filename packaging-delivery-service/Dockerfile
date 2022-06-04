FROM openjdk:8
ADD target/packaging-delivery.jar packaging-delivery.jar
EXPOSE 8083
ENTRYPOINT ["java","-jar","packaging-delivery.jar"]