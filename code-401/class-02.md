# Arrays,Loops,Imports

## Packages and Import

* Package = directory
* Java classes can be grouped together in packages
* A package name is the same as the directory (folder) name which contains the .java files.

## Package declaration

* The first statement, other than comments, in a Java source file, must be the package declaration.
* Default package. Altho all Java classes are in a directory, it's possible to omit the package declaration.

## Package declaration syntax

* The statement order is as follows. Comments can go anywhere.
  * Package statment (optional).
  * Imports (optional).
  * Class or interface definitions.

* Does importing all classes in a package make my object file (.class or .jar) larger?
  * No, import only tells the compiler where to look for symbols.
* It's hard to remember to remove classes when they are no longer used, so the import list is surprisingly often wrong. It can seriously slow down reading because unusual or unexpected class imports make me look for that class, only to discover that it must have been used in an earlier version.
* Explicit class imports permit accidentally defining classes with names that conflict with the standard library names. This is very bad. Using "*" to import all classes prevents this dangerous naming accident.

# Java Loops

*  looping is a feature which facilitates the execution of a set of instructions until the controlling Boolean-expression evaluates to false.

* Java provides different types of loops to fit any programming need. Each loop has its own purpose and a suitable use case to serve.

* Here are the types of loops that we can find in Java:
  * Simple for loop
  * Enhanced for-each loop
  * While loop
  * Do-While loop

## For Loop

* A for loop is a control structure that allows us to repeat certain operations by incrementing and evaluating a loop counter.

## While Loop

* The while loop is Java's most fundamental loop statement.
* It repeats a statement or a block of statements while its controlling Boolean-expression is true.

##  Do-While Loop

* The do-while loop works just like the while loop except for the fact that the first condition evaluation happens after the first iteration of the loop.
* 
