# HTML Text
* Structural markup: the elements that you can use to describe both headings and paragraphs.

### HTML Heading:
* HTML has six "levels" of headings:
``` html
    <h1></h1>
    <h2></h2>
    <h3></h3>
    <h4></h4>
    <h5></h5>
    <h6></h6>
    //The contents of an <h1> element is the largest, and the contents of an <h6> element is the smallest. 

```
### HTML Paragraphs
* we can create a paragraph using ```<p>``` tage.
* We can create a bold text by enclosing words in the tags ```<b> and </b>```
* We can create a italic text by enclosing words in the tags ```<i> and </i>```
* We can create a superscript text by enclosing words in the tags ```<sup> and </sup>```
* We can create a subscript text by enclosing words in the tags ```<sub> and </sub>```
* to add a line break inside the middle of a paragraph you can use the line break tag ```<br />```.
* create a horizontal rule between sections using the ```<hr />``` tag.
* The ```<strong>```element indicates that its content has strong importance and by default the browser make it bold.
* The ```<em>``` element indicates emphasis that subtly changes and by default the browser make it italic.
* we can create Quotations by 2 tags:
   * ```<blockquote>```  for longer quotes.
   * ``` <q> ``` used for shorter quotes.
* we can create Abbreviations & Acronyms by using ```<abbr>``` tag.
*  ```<cite>``` tag is referred to citation which it referencing a piece of work such as a book,film or research paper, the ```<cite>``` element can be used to indicate where the citation is from.
*  
## Semantic Markup
* Semantic markup: which some text elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages.
# Introducing CSS
* Block level elements look like they start on a new line. 
* Inline elements flow within the text and do not start on a new line.
* CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.
* there is 2 way to Associates css Style rules with HTML elements:
  * Using External CSS by ```<link>```.
  * Using Internal CSS by ```<style>```.
* CSS Selectors:There are many different types of CSS selector that allow you to target rules to specific elements in an HTML document such as :
  * Universal Selector
  * Type Selector
  * Class Selector
  * ID Selector
  * Child Selector
  * Descendant Selector
  * Adjacent Sibling Selector
  * General Sibling Selector
# Basic JavaScript Instructions
*  statement:instructions that a computer can follow one-by-one.
*  we can create comments in javascript by 2 way:
   * MULTI-LINE COMM ENTS : starting with the /* characters and ending with the */ characters.
   * SINGLE-LINE COMMENTS : anything that follows the two forward slash characters // on that line will not be processed by the JavaScript interpreter .
* variables: are a palce that we can store temporarily  bits of information or data.
* the data type :
  * String
  * number
  * boolean 
* ARRAYS:y is a special type of variable. It doesn't just store one value; it stores a list of values. 
* EXPRESSIONS: which it evaluates into (results in) a single value, there is 2 type of expressions:
    * EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE .
    * EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE .
# Decisions and Loops
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
* ```>``` :greter than <br>
  checks if the nuber on the left is greater than the number on the right.
* ```>=```  : greater than or equal to <br>
checks if the number on the left is greater than or equal to the number on the right .
## Logical Operators
* && :Logical and <br>
  test more than one condition ,if both expression to true then the expression returns true.
* || :Logical or <br>
  test  at least one condition,if either expression evaluates to true then the expression returns true.
* ! :Logical not <br>
* take a single boolean value and inverts it . 
# Loop 
> There are three types of loop: for, while, and 
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



