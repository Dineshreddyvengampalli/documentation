## What is event-loop?
In node server  whenever a request comes , these request is stored in queue. Event loop is something that picks up that request present in the queue and process it . Event loop process the single request at a time.The event loop checks wether the request that is processing is io blocking or io non-blocking.If the request is IO non-blocking it will immediately process the request and sends the response back. If the request is IO blocking, ultimately it will take some time get the response back untill the response time the event loop pushes the request to the service queue in which the status of all the requests present in the service queue are set to hold.
	  After sending the request to the service queue (if it is IO blocking) the event loops takes 
the next request form the queue and starts to process it.If the response for the perticular IO blocking request is received..then it takes the perticular request from the service queue and sents the response back to the UI.

## Need for Event-Loop
Since js is a single-threaded language , event loop enables js to resemble as multi-threaded language.Only by the use of event-loop the node server can handle IO blocking requests optimally by sending these process to the service queue ans send the response with a delay without blocking the next request in queue.To continously listen to the events and requests emitted by the user and handle them one at a time Event-Loop is required.

## Pros of Node
--> A single Programming language to learn for both front-end and back-end (js).
--> Good for developing micro services.
--> Speed and scalability

## Cons of Node
--> Cannot handle high computational apps and load on cpu
--> Meant to use only for no-sql database

## Scanarios to not to prefer Node
Since js is a single-threaded language,it handles the request form the queue one at a time . If the application required high computation and load on cpu , then it is better to choose multi-threaded language instead of node.

## Scanarios to prefer Node
The applications that are no longer needed for higher computation and load on cpu, those are prefered to use node.Since the lesser computation is required, one can design and implement highly scalable web-applications. To implement microservices that are less computational and load on cpu Node is the best option to use.
