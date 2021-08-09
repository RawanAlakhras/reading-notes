# Spring RequestMapping

* we'll focus on one of the main annotations in Spring MVC: @RequestMapping.
* the annotation is used to map web requests to Spring Controller methods.

## @RequestMapping — the HTTP Method

* The HTTP method parameter has no default. So, if we don't specify a value, it's going to map to any HTTP request.

## RequestMapping and HTTP Headers

* @RequestMapping With the headers Attribute : The mapping can be narrowed even further by specifying a header for the request .

* @RequestMapping Consumes and Produces: Mapping media types produced by a controller method is worth special attention.

* We can map a request based on its Accept header via the @RequestMapping headers

## RequestMapping With Path Variables

* Parts of the mapping URI can be bound to variables via the @PathVariable annotation.
* If the name of the method parameter matches the name of the path variable exactly, then this can be simplified by using @PathVariable with no value.

*  Multiple @PathVariable : A more complex URI may need to map multiple parts of the URI to multiple values.
* @PathVariable With Regex : Regular expressions can also be used when mapping the @PathVariable.

## RequestMapping With Request Parameters

* @RequestMapping allows easy mapping of URL parameters with the @RequestParam annotation.

We are now mapping a request to a URI:
* @RequestMapping can optionally define the parameters as yet another way of narrowing the request mapping:

## RequestMapping Corner Cases

* @RequestMapping — Multiple Paths Mapped to the Same Controller Method
* a single @RequestMapping path value is usually used for a single controller method (just good practice, not a hard and fast rule),
* there are some cases where mapping multiple requests to the same method may be necessary.
* In that case, the value attribute of @RequestMapping does accept multiple mappings, not just a single one.

## Ambiguous Mapping Error

* The ambiguous mapping error occurs when Spring evaluates two or more request mappings to be the same for different controller methods.
* A request mapping is the same when it has the same HTTP method,URL, parameters, headers, and media type.

## New Request Mapping Shortcuts

* Spring Framework 4.3 introduced a few new HTTP mapping annotations, all based on @RequestMapping:
* @GetMapping
* @PostMapping
* @PutMapping
* @DeleteMapping
* @PatchMapping

## Accessing Data with JPA

*  the process of building an application that uses Spring Data JPA to store and retrieve data in a relational database.

## What You need

* A favorite text editor or IDE
* JDK 1.8 or later
* Gradle 4+ or Maven 3.2+

## Starting with Spring Initializr

* visit the [Spring Initializr](https://start.spring.io/) to generate a new project with the required dependencies (JPA and H2).

## Define a Simple Entity

* Starts by defining a class with it's members and constructor including getters and setters if wanted .
* Then You have to annotate the class with @Entity annotation .
* After that start by adding an id as a data member annotated with @Id and @GeneratedValue with (strategy = GenerationType.Auto) This means that the id value will be generated automatically .
* In entity the default constructor must be declared .
* The arg-Constructor is used to create objects and save in the database .

## Create Simple Queries

* Spring Data JPA focuses on using JPA to store data in a relational database.
* Its most compelling feature is the ability to create repository implementations automatically, at runtime, from a repository interface.
* CustomerRepository extends the CrudRepository interface.
* The type of entity and ID that it works with, Customer and Long, are specified in the generic parameters on CrudRepository.
* By extending CrudRepository, CustomerRepository inherits several methods for working with Customer persistence, including methods for saving, deleting, and finding Customer entities.
* Spring Data JPA also lets you define other query methods by declaring their method signature. 

