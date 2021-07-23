# Object

* Objects group together a set of variables and functions to create a model of a something you would recognize from the real world.

* IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES .
* IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS .
* CREATING OBJECTS USING LITERAL NOTATION
  
```javascript
    var hote l = { 
name: 'Quay', 
rooms: 40, 
booked : 25, 
checkAvailability: function() { 
return this.rooms - this.booked; 
} 
} ; 
JAVASCRIPT 
var el Name = document .getElementByld('hotelName'); 
elName.textContent =hotel .name; 
var elRooms = document.getElementByid{'rooms'); 
elRooms.textContent = hotel .checkAvailability();
```

# The Document Object Model (DOM)

* The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.
* THE DOM TREE IS A MODEL OF A WEB PAGE .
* DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes. 
* 

## ACCESSING ELEMENTS

* DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes.
* METHODS THAT RETURN A SINGLE ELEMENT NODE:
  * getElementByld( "id")
  * querySelector( 'css selector')
* METHODS THAT RETURN ONE OR MORE ELEMENTS (AS A NODELIST):
  * getElementsByClassName( 'class ' )
  * getElementsByTagName( 'tagName')
  * querySelectorAll ( 'css select')

## TRAVERSING THE DOM

* When you have an element node, you can select another element in relation to it using these five properties.
* parentNode :This property finds the element node for the containing (or parent) element in the HTML. 
* previousSibling nextSibling : These properties find the previous or next sibling of a node if there are siblings. 
* first Child lastChild:These properties find the first or last child of the current element. 
* From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques. 
* An element node can contain multiple text nodes and child elements that are siblings of each other. 
* In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery). 
* Browsers offer tools for viewing the DOM tree . 

