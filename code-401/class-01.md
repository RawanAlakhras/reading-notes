# Java Basics

## Variables

* basic data types (primitive types, character strings, and arrays)
* The Java programming language defines the following kinds of variables:
  * Instance Variables (Non-Static Fields) Technically speaking, objects store their individual states in "non-static fields", that is, fields declared without the static keyword. Non-static fields are also known as instance variables because their values are unique to each instance of a class (to each object, in other words); the currentSpeed of one bicycle is independent from the currentSpeed of another.
  * Class Variables (Static Fields) A class variable is any field declared with the static modifier; this tells the compiler that there is exactly one copy of this variable in existence, regardless of how many times the class has been instantiated.
  * Local Variables Similar to how an object stores its state in fields, a method will often store its temporary state in local variables.
  * Parameters You've already seen examples of parameters, both in the Bicycle class and in the main method of the "Hello World!" application.
* The rules and conventions for naming your variables can be summarized as follows:
  * Variable names are case-sensitive.
  * Subsequent characters may be letters, digits, dollar signs, or underscore characters.
  * If the name you choose consists of only one word, spell that word in all lowercase letters.

## Operators

* Operators are special symbols that perform specific operations on one, two, or three operands, and then return a result.

## Expressions, Statements, and Blocks

* expressions are the core components of statements; statements may be grouped into blocks.
* Expressions: An expression is a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value.
* The data type of the value returned by an expression depends on the elements used in the expression.
* The Java programming language allows you to construct compound expressions from various smaller expressions as long as the data type required by one part of the expression matches the data type of the other.
* Statements : Statements are roughly equivalent to sentences in natural languages. A statement forms a complete unit of execution. The following types of expressions can be made into a statement by terminating the expression with a semicolon (;).
* Blocks: A block is a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed

## Control Flow Statements

* The statements inside your source files are generally executed from top to bottom, in the order that they appear.
* Control flow statements, however, break up the flow of execution by employing decision making, looping, and branching, enabling your program to conditionally execute particular blocks of code.

# Reddit thread on compiling

* What does it mean to compile code?
  * When you compile code, the compilor (usually another program) takes the program the human wrote, and converts it into the program the computer can understand


