# State and Props
* Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?<br>
‘render’ happens first .
* What is the very first thing to happen in the lifecycle of React?<br>
the mounting phase .
* Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates.
1. constructor
2. render
3.  componentDidMount
4. React Updates
5. componentWillUnmount
* What does componentDidMount do?<br>
`componentDidMount()`
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions.

