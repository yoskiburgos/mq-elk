FROM maven:3.6-jdk-8-alpine
COPY pom.xml /app/
COPY src /app/src
RUN cd /app && mvn -e -B package
ENTRYPOINT ["java", "-jar", "/app/target/colasMQ-0.1.jar"]
EXPOSE 8089

#usar solo jar
