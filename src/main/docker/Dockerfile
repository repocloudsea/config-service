FROM frolvlad/alpine-oraclejdk8:slim
ADD cls-config-service-0.0.1-SNAPSHOT.jar cls-config-service-0.0.1-SNAPSHOT.jar
RUN sh -c 'touch /cls-config-service-0.0.1-SNAPSHOT.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /cls-config-service-0.0.1-SNAPSHOT.jar" ]
EXPOSE 9001