# API-gateway

## Development environment

**Spring Cloud Gateway —** Enable our project to be a Cloud API gateway

**Eureka Discovery Client —** Enable our project to be discovered by a Eureka server and allow our services to communicate with this service in a seamless way.

**Spring Boot Actuator —**  To enable our project to be monitored by the EUREKA server and any other monitoring tools will be able to ping this service’s uptime.

 Service is running on docker, image specified in docker-compose.yml file, and started by docker-compose.
 
 we are mapping Spring Cloud Gateway to our menusync service, any request that starts with a http://localhost:8081/menu will redirect to the menySync-service.
 
## Reason to choose Cloud Gateway
So, in this case, I've named the service Zuul-service, but in truth, I've used Spring Cloud Gateway. The primary reason for this is that Zuul is built on servlet 2.5 (works with 3.x) , using blocking APIs. It does not support long-lived connections such as websockets.


Gateway is built with non-blocking APIs on Spring Framework 5, Project Reactor, and Spring Boot 2.  Websockets are supported, and it's a much better developer experience and provides a flexible way of routing requests based on a number of criteria.
 
