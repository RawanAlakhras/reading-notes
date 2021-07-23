# Lists 
* HTML have three different types of lists:
   1. Ordered lists :are lists where each item in the list is numbered. `<ol>`
   2. Unordered lists : are lists that begin with a bullet point .`<ul`
   3. Definition lists : are made up of a set of terms along with the definitions for each of those terms.`<dl>`
* Lists can be nested inside one another.
# Boxes
* box have Dimensions (width & height).
# Overflowing Content
* overflow: it is a property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:
   1. hidden: This property simply hides any extra content that does not fit in the box.
   2. scroll: This property adds a scrollbar to the box so that users can scroll to see the missing content.
* Every box has three available properties that can be adjusted to control its appearance:
   1. Border: it is separates the edge of one box from another.
   2. Margin: is a sit outside the edge of the border. 
   3. Padding: is the space between the border of a box and any content contained within it.
# display:
* The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page.
* The values this property can take are:
   1. inline :This causes a block-level element to act like an inline element.
   2. block : This causes an inline element to act like a block-level element.
   3. inline-block :This causes a block-level element to flow like an inline element, 
   4. none:This hides an element from the page. 
* visibility: it is property allows you to hide boxes from users but It leaves a space where the element would have been. it have two value :
   1. hidden
   2. visible
* Box Shadows: it is a  property allows you to add a drop shadow around a box. 
* border-radius: it is a rounded corners on a box.
* The value indicates the size of the radius in pixels. 
# ARRAYS
* An array is a special type of variable. It doesn't just store one value; it stores a list of values. 
  
```javascript
    var colors; 
    colors ['white', 'black', ' custom']; 
```

* Values in an array are accessed as if they are in a numbered list.
# Decisions and Loops
* Conditional statements allow your code to make decisions about what to do next. 
*  if statement: 
  
```javascript
    if(1 >2 ){

    }
    else{

    }
```

* Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>) are used to compare two operands. 
## Comparison Operators
* == :is Equal to <br>
  this operator comares tow values to see if they are the same.
 * === :strict equal to<br>
  compares two values to chech that both the data type and value are the same.
* != :is not equal to <br>
  this operator compares tow values to see if they are not the same .
* !== :strict not equal to <br>
  compares two values to check that both the data type and value are not the same .
* < :less than <br>
  checks if the number on the left is less than the number on the right .
* <= : less than or equal to <br>
  checks if the number on the left is less than or equal to the number on the right .
* `>` :greter than <br>
  checks if the nuber on the left is greater than the number on the right.
* `>=`  : greater than or equal to <br>
checks if the number on the left is greater than or equal to the number on the right .
# Logical operators 
* allow you to combine more than one set of comparison operators.
* && :Logical and <br>
  test more than one condition ,if both expression to true then the expression returns true.
* || :Logical or <br>
  test  at least one condition,if either expression evaluates to true then the expression returns true.
* ! :Logical not <br>
* take a single boolean value and inverts it . 

>Comparison Operators & Logical operators are Quotes from class-02 for reading-notes in the same repo.

## SWITCH STATEMENTS 
* A switch statement starts with a variable called the switch value.
* Each case indicates a possible value for this variable and the code that should run if the variable matches that value. 
# Loop 
 There are three types of loop: for, while, and 
do ... while. Each repeats a set of statements.
### FOR 
if you need to run code a specific number of times .
``` javascript
    for (var i = 0 ; i<10 ;i++)
    {

    }
```

### WHILE 
If you don't know how many times the code should run 
```javascript 
    while(condition ){
        do something
    }
```

### do-while
it will always run the statement at least once,even if the condition evaluates to false .
```javascript 
    do {
    
    }while(condition);
```

>LOOP SECTION Quotes from class-02 for reading-notes in the same repo.


