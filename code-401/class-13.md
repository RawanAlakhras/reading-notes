# Related data in Spring

## One-to-One Relationship

* define two entity classes Library and Address having a one-to-one relationship,
* using the @OneToOne annotation. The association is owned by the Library end of the association:
* The @RestResource annotation is optional and can be used to customize the endpoint.
* We must be careful to have different names for each association resource
* The association name defaults to the property name and can be customized using the rel attribute of @RestResource annotation:
* If we were to add the secondaryAddress property above to the Library class, we would have two resources named address, and we would encounter a conflict.
* In order to expose these entities as resources,we need to create two repository interfaces for each of them, by extending the CrudRepository interface
* Sending get request to an endpoint would return an empty object if no post requests was sent.
* We use the PUT method to retrieve the JSON object or Delete to delete a record.

## One-to-Many RelationShip

* A one-to-many relationship is defined using the @OneToMany and @ManyToOne annotations and can have the optional @RestResource annotation to customize the association resource.
* To remove an association, we can use the DELETE method on the association resource:
* to Expose it we need the same repository interface that extends CRUDRepository.
* Use the PUT request to associate the repository with the association.

## Many-to-Many Relationship

* A many-to-many relationship is defined using @ManyToMany annotation, to which we can add @RestResource.
* we need to create a repository interface to manage the entity.
* we need to sending a POST requests to the collection resource.
*  we can send a GET request to the association endpoint to verify both entity have been associated.
* To remove an association, we can send a request with DELETE method to the URL of the association resource

## Testing the Endpoints With TestRestTemplate

* Define a class that injects a TestRestTemplate.
* Define the endpoints as strings.
* Declare @Test method to start testing.
* Make an object for each class you want to test the relation on.
* Use postEntity to the specific objects.
* use the HttpHeaders to add the headers of the request.
* assertEquals the response for each.

# Integration Testing in Spring

## Preparation

* Several Maven dependencies are required for running the integration tests

## Spring MVC Test Configuration

* Enable Spring in Tests with JUnit 5:JUnit 5 defines an extension interface through which classes can integrate with the JUnit test.
* We can enable this extension by adding the @ExtendWith annotation to our test classes and specifying the extension class to load. 
* To run the Spring test, we use SpringExtension.class.
* We also need the @ContextConfiguration annotation to load the context configuration and bootstrap the context that our test will use.
* in @ContextConfiguration, we provide the ApplicationConfig.class config class, which loads the configuration we need for this particular test.
* We use a Java configuration class here to specify the context configuration. Similarly, we can use the XML-based configuration:
* Finally, we also annotate the test with @WebAppConfiguration, which will load the web application context.


## The WebApplicationContext Object

* WebApplicationContext provides a web application configuration. It loads all the application beans and controllers into the context.
* MockMvc provides support for Spring MVC testing. It encapsulates all web application beans and makes them available for testing.
* We initialize the mockMvc object in the @BeforeEach annotated method so that we don't have to initialize it inside every test.
* Let's verify that we're loading the WebApplicationContext object (webApplicationContext) properly. We'll also check that the right servletContext is being attached:

