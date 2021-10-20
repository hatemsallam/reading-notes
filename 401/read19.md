# Spring and Sockets

* WebSocket is a thin, lightweight layer above TCP.
* This makes it suitable for using “subprotocols” to embed messages.
* STOMP messaging: is a subprotocol operating on top of the lower-level WebSocket.

* we can use WebSocket to build a server that accepts a message that carries a user’s name. In response, the server will push a greeting into a queue to which the client is subscribed.


## Requirement

* A favorite text editor or IDE
* JDK 1.8 or later
* Gradle 4+ or Maven 3.2+

## how we can build a server that accepts a message that carries a user’s name ??

1. visit the [Spring Initializr](https://start.spring.io/) to generate a new project with the required dependency (Websocket).
2. add websocket dependencies .
3. Create a Resource Representation Class
    * create your STOMP message service
    * The service will accept messages that contain a name in a STOMP message whose body is a JSON object.
    * To model the message you can create a plain old Java object with a name property and a corresponding getName() method.
    * the service will process it by creating a greeting and publishing that greeting on a separate queue to which the client is subscribed. 
    * The greeting will also be a JSON object
    * Spring will use the Jackson JSON library to automatically marshal instances of type Greeting into JSON.
4. Create a Message-handling Controller
    * STOMP messages can be routed to @Controller classes.
    * The @MessageMapping annotation ensures that, if a message is sent to the /hello destination, the greeting() method is called.
    * The payload of the message is bound to a HelloMessage object which is passed into greeting().
    * the implementation of the method simulates a processing delay by causing the thread to sleep for one second. 
    * after the client sends a message, the server can take as long as it needs to asynchronously process the message.
    * The client can continue with whatever work it needs to do without waiting for the response.
    * After the one-second delay, the greeting() method creates a Greeting object and returns it. 
    * The return value is broadcast to all subscribers of /topic/greetings, as specified in the @SendTo annotation. 
5. Configure Spring for STOMP messaging
    * configure Spring to enable WebSocket and STOMP messaging.
    * Create a Java class named WebSocketConfig
    * WebSocketConfig is annotated with @Configuration to indicate that it is a Spring configuration class.
    * It is also annotated with @EnableWebSocketMessageBroker. As its name suggests, @EnableWebSocketMessageBroker enables WebSocket message handling, backed by a message broker.
6. Create a Browser Client
    * you can turn your attention to the JavaScript client that will send messages to and receive messages from the server side.
    * The connect() function uses SockJS and stomp.js to open a connection
    * he sendName() function retrieves the name entered by the user and uses the STOMP client to send
7. Make the Application Executable
    * Spring Boot creates an application class for you
    * You can use it to run this application. 