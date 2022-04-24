# Component Based UI

React is a JavaScript library, that enables us to create UIs using multiple reusable components.


## JSX

The above syntax is known as JSX, and it is a JavaScript syntax extension. It's best to use it alongside React to describe how the UI should look. JSX looks like a template language, but it has all of JavaScript's capabilities. React "elements" are created via JSX. In the next section, we'll look at how to render them to the DOM. 

**_JSX is an Expression_**

This means you may use JSX in if statements and loops, assign variables to it, receive it as arguments, and return it from functions.

**_Specifying Attributes with JSX_**

When embedding a JavaScript expression in an attribute, don't use quotations around curly braces. Either quotes (for string values) or curly braces (for expressions) should be used in the same property, but not both.

**_JSX Prevents Injection Attacks_**

It's safe to include user input in JSX since React DOM automatically escapes any values stored in JSX before rendering them. As a result, you'll never be able to inject anything that isn't expressly specified in your application. Before being rendered, everything is transformed to a string. This protects against cross-site scripting (XSS) attacks.

## Rendering Elements

What you see on the screen is described by an element. React elements, unlike browser DOM elements, are simple objects that are easy to generate. The DOM is updated to match the React elements by React DOM.

**_Rendering an Element into the DOM_**

To render a React element, first pass the DOM element to ReactDOM.createRoot(), then pass the React element to root.render():
