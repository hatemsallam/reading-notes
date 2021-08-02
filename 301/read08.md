# What does REST stand for?

In 2000, Roy Fielding proposed Representational State Transfer (REST) as an architectural approach to designing web services. REST is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP. However, most common REST API implementations use HTTP as the application protocol, and this guide focuses on designing REST APIs for HTTP.

A primary advantage of REST over HTTP is that it uses open standards, and does not bind the implementation of the API or the client applications to any specific implementation. For example, a REST web service could be written in ASP.NET, and client applications can use any language or toolset that can generate HTTP requests and parse HTTP responses.




## REST APIs are designed around a resources, which are any kind of object, data, or service that can be accessed by the client.




## What is an identifer of a resource? Give an example.

 - is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:
 
 HTTP

https://adventure-works.com/orders/1



## What are the most common HTTP verbs?

- GET, POST, PUT, PATCH, and DELETE.







## What should the URIs be based on?

- based on nouns (the resource) and not verbs (the operations on the resource).







## Give an example of a good URI.

- https://adventure-works.com/orders/1








## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?


- web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires.





## What status code does a successful GET, POST, DELETE request return?


- Sending an HTTP GET request to the collection URI retrieves a list of items in the collection. Each item in the collection also has its own unique URI. An HTTP GET request to the item's URI returns the details of that item.



## What status code does an unsuccessful GET request return?
HTTP status code 406 (Not Acceptable).









