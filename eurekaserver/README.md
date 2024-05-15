# Summary

•	We use a service discovery pattern to abstract away the physical location of our
services.

•	A service discovery engine like Eureka can seamlessly add and remove service
instances from an environment without impacting the service clients.

•	Client-side load balancing can provide an extra level of performance and resiliency
by caching the physical location of a service on the client making the service
call.

•	Eureka is a Netflix project that, when used with Spring Cloud, is easy to set up
and configure.

•	You can use these three different mechanisms in Spring Cloud and Netflix
Eureka to invoke a service: Spring Cloud Discovery Client, Spring Cloud Load
Balancer–backed RestTemplate, and Netflix’s Feign client.
