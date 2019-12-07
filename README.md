This repo is for SpringBoot microservice using SpringCloud EurekaDiscoveryService and Zull API gateway
## To run spring boot aaplication from command line and with instance id passwd from command line
mvn spring-boot:run -Dspring-boot.run.arguments=--spring.application.instance_id=pankaj
## To run spring boot microservice with a specific instance id and port number
mvn spring-boot:run -Dspring-boot.run.arguments=--spring.application.instance_id=pankaj2,--server.port=8999
