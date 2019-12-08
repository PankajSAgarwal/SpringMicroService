This repo is for SpringBoot microservice using SpringCloud EurekaDiscoveryService and Zull API gateway
## To run spring boot aaplication from command line and with instance id passwd from command line
mvn spring-boot:run -Dspring-boot.run.arguments=--spring.application.instance_id=pankaj
## To run spring boot microservice with a specific instance id and port number
mvn spring-boot:run -Dspring-boot.run.arguments=--spring.application.instance_id=pankaj2,--server.port=8999
### H2-in memory console
Add below dependency in POM in user controller service
<!-- https://mvnrepository.com/artifact/org.springframework.boot/spring-boot-starter-data-jpa -->
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-data-jpa</artifactId>
		</dependency>
		<!-- https://mvnrepository.com/artifact/com.h2database/h2 -->
		<dependency>
    		<groupId>com.h2database</groupId>
    		<artifactId>h2</artifactId>
    		<scope>runtime</scope>
	   </dependency>

You will need to start discovery service , Zuul API gateway service and use url http://192.168.29.111:8011/users-ws/h2-console
Click on "Test Connection" no password required and userid should be sa

