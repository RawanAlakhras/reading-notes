# React and Forms

* Controlled Component: In HTML, form elements such as <input>, <textarea>, and <select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React 

* Since the value attribute is set on our form element, the displayed value will always be this.state.value, making the React state the source of truth. Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.

* With a controlled component, the input’s value is always driven by the React state. 
* you can pass the value to other UI elements , or reset it from other event handlers.


# ternary operator:
* We use it because it is the shortest way

``` javascript
    x===y ? console.log(true) :console.log(false);

```