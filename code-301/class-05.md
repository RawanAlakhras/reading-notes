# Putting it all together
* How would you break a mock into a component heirarchy?<br>
The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names.
* single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.
* The easiest way is to build a version that takes your data model and renders the UI but has no interactivity. It’s best to decouple these processes because building a static version requires a lot of typing and no thinking, and adding interactivity requires a lot of thinking and not a lot of typing. We’ll see why.
* To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.
* What are the three questions you can ask to determine if something is state?<br>
1. Is it passed in from a parent via props? If so, it probably isn’t state.<br>
2. Does it remain unchanged over time? If so, it probably isn’t state.<br>
3. Can you compute it based on any other state or props in your component? If so, it isn’t state.<br>
* Identify Where Your State Should Live<br>
* Identify every component that renders something based on that state.
* Find a common owner component (a single component above all the components that need the state in the hierarchy).
* Either the common owner or another component higher up in the hierarchy should own the state.
* If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

