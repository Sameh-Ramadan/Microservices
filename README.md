# Microservices
Source : Spring Microservices in Action Book
https://github.com/ihuaylupo/manning-smia/tree/master
![Architecture](https://github.com/Sameh-Ramadan/Microservices/assets/56082179/aafb26a1-ff9b-4769-8d52-a16f32a466ab)

The client authenticates with Keycloak to get an access token. 

When token is obtained, the client makes a request to the Spring Cloud API Gateway. 

The API Gateway service communicates with the Eureka service discovery to retrieve the locations of the organization and licensing services

The API Gateway service then calls the specific microservice.

When the request arrives organization service, it validates the access token against Keycloak to see if the user has permission to continue the process. 

The organization service updates and retrieves its information from the organization database and sends it back to the client as an HTTP response.

Another path when organization information is updated, the organization service adds a message to the Kafka topic so the licensing service is aware of the change.

When the message arrives at the licensing service, Redis stores the specific information in Redis's in-memory database. 

The architecture uses distributed tracing from Zipkin, Elasticsearch, and Logstash to manage and display the logs.

And it employs Spring Boot Actuator, Prometheus, and Grafana to display the application metrics.



