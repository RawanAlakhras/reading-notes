# Spring

* build an application that has a static home page and that will also accept HTTP GET requests at: <http://localhost:8080/greeting>

* It will respond with a web page that displays HTML.

## What You Need

* A favorite text editor or IDE
* JDK 1.8 or later
* Gradle 4+ or Maven 3.2+

## Starting with Spring Initializr

* visit the [Spring Initializr](https://start.spring.io) to generate a new project with the required dependencies.
* Choose either Gradle or Maven and the language you want to use. This guide assumes that you chose Java.
* Click Dependencies and select Spring Web, Thymeleaf, and Spring Boot DevTools.
* Click Generate.
* Download the resulting ZIP file, which is an archive of a web application that is configured with your choices.

## Create a Web Controller

* In Spring’s approach to building web sites, HTTP requests are handled by a controller. 
* You can easily identify the controller by the @Controller annotation.
* A View is responsible for rendering the HTML content.
* The @GetMapping annotation ensures that HTTP GET requests to /greeting are mapped to the greeting() method.
* @RequestParam binds the value of the query string parameter name into the name parameter of the greeting() method. This query string parameter is not required.
*  Thymeleaf: is a view technology to perform server-side rendering of the HTML. 
* Thymeleaf parses the greeting.html template and evaluates the th:text expression to render the value of the ${name} parameter that was set in the controller.


## Spring Boot Devtools

* Enables hot swapping.
* Switches template engines to disable caching.
* Enables LiveReload to automatically refresh the browser.
* Other reasonable defaults based on development instead of production.

## Run the Application

* You can run the application from the command line with Gradle or Maven.
* you can run the application by using ./gradlew bootRun  
*  you can build the JAR file by using ./gradlew build

## Testing Application :

* Testing the App can be easilty Done using the web browser after running the application by visit http://localhost:8080

## Adding HomePage :

* Static resources, including HTML and JavaScript and CSS, can be served from your Spring Boot application by dropping them into the right place in the source code. 
* y default, Spring Boot serves static content from resources in the classpath at /static


## Spring model attributes

* Spring MVC calls the pieces of data that can be accessed during the execution of views model attributes. 
* The equivalent term in Thymeleaf language is context variables.
* There are several ways of adding model attributes to a view in Spring MVC.
    * Add attribute to Model via its addAttribute method:
    * By returning Model and view object by the method .
    * Using @ModelAttribute which will return all the attributes in the message Repository .
* All these attributes can be accessed by thymeleaf templates .
* Model attributes can be accessed from thymeleaf by the following syntax ${attribute name} .
* You can access request parameters easily from thyme leaf using param prefix .