#继承centos docker file
FROM centos

#安装JDK
RUN yum install -y java

#配置docker存储目录
VOLUME /tmp

#将maven目录的jar包拷贝到docker中，并命名为for_docker.jar
ADD maven/spring-boot-mongodb-0.0.1-SNAPSHOT.jar spring-boot-mongodb-demo.jar

ENTRYPOINT ["java", "-jar", "/spring-boot-mongodb-demo.jar"]