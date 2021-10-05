# HTTP Requests 

### - Step 1 : Local proccesing :
    - The browser extracts the protocol and resource path in addition to optional port with string params .
    - Form for Request is : <protocol>://<host><:optional port>/<path/to/resource><?query> .
    - Then the browser needs to resolve an IP address for your request using you os cache , DNS cache .

### - Step 2 : Resolve an IP :
    - Resolving an IP requires many steps using the DNS server with many fallovers when a request is failed .
    - If the cache search fails the DNS will fire a UDP Request which will pass through many networks and servers to find your IP .
    - The device will use a table to determine which networks are there .
    - The DNS keeps passing requests to other DNS servers until it finds the requested address or throw an error if it finds a closed or dead end .
    - The request returns a reeponse with information held by the response IP address and the time it will be cached .

### - Step 3 : Establish a TCP connection :
    - Major differ between TCP AND UDP is that TCP ensures data transmission and delivery of data .
    - TCP works using a method called three way hand shake which works as the following : 
        - The client sends a SYN packet to the server initialized randomly .
        - The server respones with SYN-ACK .
        - The client server sends an SYN with x+1 which will match the ack packet .

    - These processes are known as full duplex communication .

### - Step 4 : Send an HTTP Request : 
    - The HTTP request contains header and body .
    - It holds the HTTP method to be requested with the request line including the port or the ip it is sent over .
    - The HTTP request have a JSON format or form data more often .
    - Once the request is sent it follows the TCP procedures which will ensure the fully transmission of the request .
    - When the request is received the server returns a response with the same request line with the status additional .
    - The TCP will re order the response packets as required .

### Step 5 : Tearing down and cleaning up : 
    - The client send a FYN packet and recieves an ACK packet to prevent delayed packets from being lost .
    - After that your browser will start to fetch the data received to the requested format or extension for example shows an HTML page .


## Example request in java : 

- We use built in java class HTTPUrlConnection to establish connection (HttpClientApi in JDK 11) .

- The built in class can help us in performing basic Web requests without using additional libraries .

- We use the openConnection method to create a connection method .

- Method setRequestType is used to set the type of the request that we want to establish .

- To add request parameters we should set doProperty to true and use the outPutStream to send a getoutputstream method to it's constructor .

- We use setRequestProperty to set the request head , getHeaderField will read the header of the request .

- setConnectionTimeout , setReadTimeout are used to set timeouts to the request .

- We can parse cookies using HTTPCookie.parse method .

- After parsing cookies we can add them to the cookiestore using the add method .

- To handle the redirects we use setInstanceFollowRedirects method for a specific connection setFollowRedirects for all connections .

- We use input stream reader method to read the response of the request and we use getResponseCode to get the status of the response .