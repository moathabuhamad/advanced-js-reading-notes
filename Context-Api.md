# Context API

Context provides a way to pass data through the component tree without having to pass props down manually at every level.


In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.


React.createContext() is all you need. It returns a consumer and a provider. The provider is a component that as its name suggests provides the state to its children. It will hold the "store" and be the parent of all the components that might need that store. Consumer as it so happens is a component that consumes and uses the state. 

When to Use Context
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop to style the Button component:

Building blocks and API
The Context API consists of some building blocks that we must know about what they are called but also what their role is:

* context, the context object is an object holding the current context value and can be subscribed to
* provider, This is a React component that provides the value in question, it grabs it from the context object
* consumer, This is a React component that can consume the value provided by the Provider and can show the value

Context vs. Redux
Context does not have dev tools currently
Redux USES context behind the scenes
The new context does not include anything like reducers, actions, or middleware
If all you are using redux for is glorified prop-drilling, then you can likely replace it with the context 
