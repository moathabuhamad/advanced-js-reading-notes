# Component Based UI

React is a JavaScript library, that enables us to create UIs using multiple reusable components.


## JSX

above syntax is called JSX, and it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript. JSX produces React “elements”. We will explore rendering them to the DOM in the next section. Below, you can find the basics of JSX necessary to get you started.


**_JSX is an Expression Too_**

This means that you can use JSX inside of if statements and for loops, assign it to variables, accept it as arguments, and return it from functions


**_Specifying Attributes with JSX_**

Don’t put quotes around curly braces when embedding a JavaScript expression in an attribute. You should either use quotes (for string values) or curly braces (for expressions), but not both in the same attribute. `remember to use camelCase`



**_JSX Prevents Injection Attacks_**

It is safe to embed user input in JSX, by default, React DOM escapes any values embedded in JSX before rendering them. Thus it ensures that you can never inject anything that’s not explicitly written in your application. Everything is converted to a string before being rendered. This helps prevent XSS (cross-site-scripting) attacks.

## Rendering Elements

an element describes what you see on the screen, Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

**_Rendering an Element into the DOM_**

To render a React element, first pass the DOM element to ReactDOM.createRoot(), then pass the React element to root.render():
