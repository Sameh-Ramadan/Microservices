# Summary

•	Spring Cloud makes it trivial to build a service gateway.

•	Spring Cloud Gateway contains a set of built-in Predicate and Filter Factories.

•	 Predicates are objects that allow us to check if the requests fulfill a set of given
conditions before executing or processing a request.

•	Filters allow us to modify the incoming and outgoing HTTP requests and
responses.

•	The Spring Cloud Gateway integrates with Netflix’s Eureka Server and can
automatically map services registered with Eureka to a route.

•	Using the Spring Cloud Gateway, you can manually define route mappings in
the application’s configuration files.

•	By using Spring Cloud Config Server, you can dynamically reload the route
mappings without having to restart the Gateway server.

•	Spring Cloud Gateway allows you to implement custom business logic through
filters. With Spring Cloud Gateway, you can create pre- and post-filters.

•	Pre-filters can be used to generate a correlation ID that can be injected into
every service flowing through the gateway.

•	Post-filters can be used to inject a correlation ID into every HTTP service
response back to a service client.
