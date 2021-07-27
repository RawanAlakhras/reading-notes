# Maps, primitives, File I/O

## Java Type System

* Java has a two-fold type system consisting of primitives such as:int, boolean and reference types such as Integer, Boolean.

* Every primitive type corresponds to a reference type.
* Every object contains a single value of the corresponding primitive type.

## Pros and Cons

* The decision what object is to be used is based on what application performance we try to achieve.
* how much available memory we have.
* the amount of available memory and what default values we should handle.

## Single Item Memory Footprint

* The reference types are objects,they live on the heap and are relatively slow to access.
* To get an object's internal structure, we may use the Java Object Layout tool .
* the primitive type variables have the following impact on the memory:
  * boolean – 1 bit
  * byte – 8 bits
  * short, char – 16 bits
  * int, float – 32 bits
  * long, double – 64 bits

* It turns out that a single instance of a reference type on this JVM occupies 128 bits except for Long and Double which occupy 192 bits:
  * Boolean – 128 bits
  * Byte – 128 bits
  * Short, Character – 128 bits
  * Integer, Float – 128 bits
  * Long, Double – 192 bits

## Memory Footprint for Arrays

* the types are grouped into four families with respect to how the memory m(s) depends on the number of elements s of the array:
  * long, double: m(s) = 128 + 64 s
  * short, char: m(s) = 128 + 64 [s/4]
  * byte, boolean: m(s) = 128 + 64 [s/8]
  * the rest: m(s) = 128 + 64 [s/2]

## Performance
  
* The performance of a Java code is quite a subtle issue, it depends very much on the hardware on which the code runs, on the compiler that might perform certain optimizations, on the state of the virtual machine, on the activity of other processes in the operating system.

## Default Values

* Default values of the primitive types are 0 ,for numeric types, false for the boolean type, \u0000 for the char type. For the wrapper classes, the default value is null.
* the reference types might acquire a value (null) that in some sense doesn't belong to their domains.

## Usage

* the primitive types are much faster and require much less memory.
* On the other hand, current Java language specification doesn't allow usage of primitive types in the parametrized types (generics),  in the Java collections or the Reflection API.

## Conclusion

* we illustrated that the objects in Java are slower and have a bigger memory impact than their primitive analogs.

# Exceptions

* The Java programming language uses exceptions to handle errors and other exceptional events.

## What Is an Exception?

* The term exception is shorthand for the phrase "exceptional event."
* Definition: An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions.
* When an error occurs within a method, the method creates an object and hands it off to the runtime system.
* The object, called an exception object, contains information about the error, including its type and the state of the program when the error occurred.
* Creating an exception object and handing it to the runtime system is called throwing an exception.

## The Catch or Specify Requirement

* Valid Java programming language code must honor the Catch or Specify Requirement.
* This means that code that might throw certain exceptions must be enclosed by either of the following:

  * A try statement that catches the exception. The try must provide a handler for the exception, as described in Catching and Handling Exceptions.
  * A method that specifies that it can throw the exception.

* The Three Kinds of Exceptions
  1. The first kind of exception is the checked exception. These are exceptional conditions that a well-written application should anticipate and recover from.
  2. The second kind of exception is the error. These are exceptional conditions that are external to the application, and that the application usually cannot anticipate or recover from.
  3. The third kind of exception is the runtime exception. These are exceptional conditions that are internal to the application, and that the application usually cannot anticipate or recover from. 
