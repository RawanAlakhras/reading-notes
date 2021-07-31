# Object-Oriented Programming Concepts

## What Is an Object?

* An object is a software bundle of related state and behavior. 
*  Software objects are often used to model the real-world objects that you find in everyday life. 
* Bundling code into individual software objects provides a number of benefits, including:
  * Modularity: The source code for an object can be written and maintained independently of the source code for other objects. Once created, an object can be easily passed around inside the system.
  * Information-hiding: By interacting only with an object's methods, the details of its internal implementation remain hidden from the outside world.
  * Code re-use: If an object already exists (perhaps written by another software developer), you can use that object in your program. This allows specialists to implement/test/debug complex, task-specific objects, which you can then trust to run in your own code.
  * Pluggability and debugging ease: If a particular object turns out to be problematic, you can simply remove it from your application and plug in a different object as its replacement. This is analogous to fixing mechanical problems in the real world. If a bolt breaks, you replace it, not the entire machine.

## What Is a Class?

* A class is a blueprint or prototype from which objects are created.

## What Is Inheritance?

* Inheritance provides a powerful and natural mechanism for organizing and structuring your software. 
* Different kinds of objects often have a certain amount in common with each other. 
* Object-oriented programming allows classes to inherit commonly used state and behavior from other classes.
* In the Java programming language, each class is allowed to have one direct superclass, and each superclass has the potential for an unlimited number of subclasses.

## What Is an Interface?

* An interface is a contract between a class and the outside world.
* When a class implements an interface, it promises to provide the behavior published by that interface. 
* Implementing an interface allows a class to become more formal about the behavior it promises to provide

## What Is a Package?

* A package is a namespace for organizing classes and interfaces in a logical manner. 
*  Placing your code into packages makes large software projects easier to manage. 
* The Java platform provides an enormous class library (a set of packages) suitable for use in your own applications. 
* This library is known as the "Application Programming Interface", or "API" for short. 
* Its packages represent the tasks most commonly associated with general-purpose programming. 
* The Java Platform API Specification contains the complete listing for all packages, interfaces, classes, fields, and methods supplied by the Java SE platform. 
