# API-gateway

## Development environment

**Spring Cloud Gateway —** Enable our project to be a ZUUL API gateway

**Eureka Discovery Client —** Enable our project to be discovered by a Eureka server and allow our services to communicate with this service in a seamless way.

**Spring Boot Actuator —**  To enable our project to be monitored by the EUREKA server and any other monitoring tools will be able to ping this service’s uptime.

 Service is running on docker, image specified in docker-compose.yml file, and started by docker-compose.
 
 we are mapping Spring Cloud Gateway to our menusync service, any request that starts with a http://localhost:8081/menu will redirect to the menySync-service.
 
