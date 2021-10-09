# Spring 

- Building a spring Application that runs on port 8080 .
- Can handle requests and response a HTML page .

### Requirements :

- An IDE or text editor .
- Gradle v4+ , maven 3.2 .
- JDK 1.8 or higher .


### Starting with spring initializer :

- Launch start.spring.io to Land on the home page .
- Specify Project ,team ,package names .
- Specify the language and version .
- Inject dependencies .
- Click on generate .
- Download the zip file which will contain your initialized project .


### Web controller :

- In spring web pages and requests are handled by the controller which is implemented using the @Controller annotation .

- @GetMapping is used to ensure that the request is mapped to the followed method which will return or process the response .

- @ReqParam is used to add request parameters which are added to a model to be accessed from the views .

- The implementation of the request methods depends on the view technology used .


### Running the application :

- You can run the application right from the IDE .

- Or you can run it from the command line using gradle bootRun command or build it also .

- You can create JAR File using java -jar command and then run it .

- You can also run the project using maven Commands .


### Testing Application :

- Testing the App can be easilty Done using the web browser after running the application .

- The default port for tom cat is 8080 .

- Use this url to test the application with the provided requests : http://localhost:8080/ .


### Adding HomePage : 

- The index.html is special file located at the static directory and will be shown at the root of the pages .

- Static directories hold the HTML , CSS , JS files .

- Spring can handle all type of static and dynamic files in your project .



## Thymeleaf 

- Adding Model attributes can be done in several ways : 
    - Using Model passed as a parameter to the request method then the attribute is added using addAttribute method .
    - By returning Model and view object by the method .
    - Using @ModelAttribute which will return all the attributes in the message Repository .

- All these attributes can be accessed by thymeleaf templates .

- Model attributes can be accessed from thymeleaf by the following syntax ${attribute name} .

- You can access request parameters easily from thyme leaf using param prefix .

- When multivalued param is passed will return a serialized array until the unless condition .

- #request is also a good approach to access request parameters .

- Adding HTTPSession object to the parameters of the request method will make it accesible from thymeleaf using the session prefix .

- Servlet contexts are shared between requests and sessions and can be accessed using #servletContext prefix .

- Accessing Spring beans can be easily done using @beanname syntax .