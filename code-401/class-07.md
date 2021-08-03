# OO Design

# SOLID: The First 5 Principles of Object Oriented Design

SOLID stands for:

* S - Single-responsiblity Principle
* O - Open-closed Principle
* L - Liskov Substitution Principle
* I - Interface Segregation Principle
* D - Dependency Inversion Principle

## Single-Responsibility Principle

* A class should have one and only one reason to change, meaning that a class should have only one job.

## Open-Closed Principle

* Objects or entities should be open for extension but closed for modification.
* This means that a class should be extendable without modifying the class itself.

## Liskov Substitution Principle

* Let q(x) be a property provable about objects of x of type T. Then q(y) should be provable for objects y of type S where S is a subtype of T.
* This means that every subclass or derived class should be substitutable for their base or parent class.

## Interface Segregation Principle

* A client should never be forced to implement an interface that it doesn’t use, or clients shouldn’t be forced to depend on methods they do not use.

## Dependency Inversion Principle

* Entities must depend on abstractions, not on concretions. It states that the high-level module must not depend on the low-level module, but they should depend on abstractions.
* This principle allows for decoupling.


# The SOLID Principles in Real Life


* the single responsibility principle (srp) asserts that a class or module should do one thing only.
* this is kind of subjective, so the principle is reinforced with the heuristic that the class or module should have only one reason to change.
* the open/closed principle states that code entities should be open for extension, but closed for modification.
* to put this more concretely, you should write a class that does what it needs to flawlessly and not assuming that people should come in and change it later. it's closed for modification, but it can be extended by, for instance, inheriting from it and overriding or extending certain behaviors.
* the liskov substitution principle (lsp) is the one here that is most unique to object-oriented programming.
* the lsp says, basically, that any child type of a parent type should be able to stand in for that parent without things blowing up.
* the interface segregation principle (isp) says that you should favor many, smaller, client-specific interfaces over one larger, more monolithic interface.
* in short, you don't want to force clients to depend on things they don't actually need.
* the dependency inversion principle (dip) encourages you to write code that depends upon abstractions rather than upon concrete details.
* you can recognize this in the code you read by looking for a class or method that takes something generic like "stream" and performs operations on it, as opposed to instantiating a specific filestream or stringstream or whatever. this gives the code in question a lot more flexibility -- you can swap in anything that conforms to the stream abstraction and it will still work.
