EDA uses events to trigger or communicate between decoupled services (microservices).In the modern application development the communication of microservices are done through event-driven architecture.
ex usecase : In an e-commerce application, lets consider 2 microservices that are placing an order and tracking the shipment.Placing an order is an event produced by the user and this event will trigger the microservice regarding order-placement.
here, placing an order is a producer and perticular microservice is a consumer.Similarly, tracking the shipment is a microservice that gets triggered or communicated by other event.

Event-driven architectures have three key components: event producers, event routers, and event consumers. A producer publishes an event to the router, which filters and pushes the events to consumers. Producer services and consumer services are decoupled, which allows them to be scaled, updated, and deployed independently.

##  Example architecture : 
![[Pasted image 20230122223318.png]]