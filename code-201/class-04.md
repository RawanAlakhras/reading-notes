# Links
* Links are created using the `<a>` element.
* The `<a>` element uses the href attribute to indicate the page you are linking to.
* If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.
* You can create links to open email programs with an email address in the "to" field.
* You can use the id attribute to target elements within a page that can be linked to.
  
# Layout
* CSS treats each HTML element as if it is in its own box. This box will either be a block-levelbox or an inline box. 
   * Block-level elements start on a new line.
   * Inline elements flow in between surrounding text .
* Containing Elements: If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.
* Controlling the Position of Elements:CSS has the following positioning schemes that allow you to control the layout of a page: 
   * Normal flow:Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. 
   * Relative Positioning:This moves an element from the position it would be in normal flow, shifting it to the top,right, bottom, or left of where it would have been placed.
   * Absolute positioning:This positions the element in relation to its containing element. 
* Floating Elements: Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box.
* When you move any element from normal flow, boxes can overlap. The z-index property allows you to control which box appears on top.
# Functions, Methods, and Objects
* FUNCTIONS & METHODS :Functions consist of a series of statements that have been grouped together because they perform a specific task.
  * creat a function 
  
```javascript
  function sayHello(){
      document.write("hello");
  }

```


   * calling a function
  
```javascript
  sayhello();
```

### ANONYMOUS FUNCTIONS & FUNCTION EXPRESSIONS 
* FUNCTION DECLARATION: creates a function that you can call later in your code.
* FUNCTION EXPRESSION: If you put a function where the interpreter would expect to see an expression, then it is treated as an expression, and it is known as a function expression. 
## VARIABLE SCOPE
* The location where you declare a variable will affect where it can be used within your code.
* LOCAL VARIABLES :When a variable is created inside a function using the var keyword, it can only be used in that function. 
* GLOBAL VARIABLES :If you create a variable outside of a function, then it can be used anywhere within the script. 
### HOW MEMORY & VARIABLES WORK 
* Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded.
* Local variables are only remembered during the period of time that a function is being executed. 
# 6 Reasons for Pair Programming
* pair programming is the practice of two developers sharing a single workstation to interactively tackle a coding task together. 
### How does pair programming work?
* pair programming commonly involves two roles: the Driver and the Navigator.
    * The Driver is the programmer who is typing and the only one whose hands are on the keyboard.
    * The Navigator uses their words to guide the Driver but does not provide any direct input to the computer.
    * 
  