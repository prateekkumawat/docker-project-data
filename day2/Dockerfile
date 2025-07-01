# Java app on redhat 
FROM redhat/ubi9:latest

# Build java and maven packages
RUN yum install -y java-17-openjdk*
RUN yum install -y maven

# create source code directory  
RUN mkdir /opt/app 

# Always work in directory
WORKDIR /opt/app 

# copy source code in image 
COPY src /opt/app/src
COPY pom.xml /opt/app 

# source code build using maven 
RUN mvn clean package -DskipTests

# RUN jar 
#CMD ["java", "-jar", "/opt/app/target/demo-0.0.1-SNAPSHOT.jar"]

EXPOSE 8080