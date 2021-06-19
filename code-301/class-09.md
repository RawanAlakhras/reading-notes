# FUNCTIONAL PROGRAMMING

* Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data .

## What is a pure function?

* When learning functional programming the first thing you need to know is oure functions and it's restricts :
  * It returns the same result if given the same arguments (it is also referred as deterministic) .
  * It does not cause any observable side effects .
  * For example when calculating datat that is external and changeable , or reading from files which will be  changed this will be impure function .
  * Random number generator also can't be pure .
  * mutability is discouraged in functional programming .
  * A function that edits data or causes changes on global variable is impure to fix that don't change the variable just return the value .

## What is Immutability?

* The second thing functional programming is about is Immutability,When data is Immutable the state of data   will not change, instead we will create a new object of it containing the new data ,To handle the iteration muatbility we use recursion which will call a function and the function will call it self several times .
* pure functions + immutable data = referential transparency
