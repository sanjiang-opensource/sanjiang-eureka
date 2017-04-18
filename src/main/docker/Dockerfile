FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD sanjiang-eureka-1.0.0.SNAPSHOT.jar sanjiang-eureka.jar
RUN sh -c 'touch /sanjiang-eureka.jar'
ENV JAVA_OPTS=""
ENTRYPOINT ["sh","-c","java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /sanjiang-eureka.jar"]