FROM adoptopenjdk/openjdk11:latest
VOLUME /tmp
ADD target/*.jar app.jar
EXPOSE 8090
ENV JAVA_OPTS=""
ENTRYPOINT ["sh", "-c", "java $JAVA_OPTS -jar /app.jar"]