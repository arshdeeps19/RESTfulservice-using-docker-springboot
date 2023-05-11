FROM openjdk:8-jdk-alpine
RUN mkdir -p /etc/arsh/
COPY customers.json /etc/arsh/customers.json
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","/app.jar"]
