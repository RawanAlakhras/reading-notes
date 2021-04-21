# Form

* There are several types of form controls that you can use to collect information from visitors to your site:
  * ADDING TEXT
  * Making Choices
  * Submitting Forms
  * Uploading Files
* Form Structure:Form controls live inside a `<form>`element. This element should always carry the action attribute and will usually have a method and id attribute too.
* action:action attribute: Its value is the URL for the page on the server that will receive the information in the form when it is submitted.
* method: Forms can be sent using one of two methods: get or post.
* Information from a form is sent in name/value pairs.
* Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server.
* HTML5 introduces new form elements which make it easier for visitors to fill in forms.

# Lists, Tables & Forms

* List markers can be given different appearances using the list-style-type and list-style image properties.
* Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.
* Forms are easier to use if the form controls are vertically aligned using CSS.
* Forms benefit from styles that make them feel more interactive

# EVENT

* There are three types of event handlers:
  * HTML EVENT HANDLERS:`<a onclick="hide()">`
  * TRADITIONAL DOM EVENT HANDLERS : DOM event handlers were introduced in the original specification for the DOM
            `element .onevent =functionName ;`

  * DOM LEVEL 2 EVENT LISTENERS :these newer event listeners allow one event to trigger multiple functions.

* EVENT LISTENERS:Event listeners are a more recent approach to handling events. They can deal with more than one function at a time .
  `element .addEventlistener('event', functionName [, Boolean]) ;`

* THE EVENT OBJECT:When an event occurs, the event object tells you information about the event, and the element it happened upon.

* Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked). 
* Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon. 
* When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user. 

