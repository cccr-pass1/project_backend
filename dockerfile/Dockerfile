FROM openjdk:17-jdk 
CMD ["./gradlew","clean","build"]
COPY build/libs/localkoreabackend_new-0.0.1-SNAPSHOT.jar app.jar
EXPOSE 8081
ENTRYPOINT ["java","-jar","/app.jar"]
