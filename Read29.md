# Advanced State with Reducers

The useReducer() hook in React allows you to decouple the component's state management from its rendering logic.

`const [state, dispatch] = useReducer(reducer, initialState)`

 **Accepts 2 argument:** 
 + The reducer function 
 + The initial state. 

## When to use useReducer?

useReducer is typically recommended over useState when you have sophisticated state logic involving several sub-values or when the future state is reliant on the prior one. UseReducer can help you increase speed for components that trigger deep updates by allowing you to pass dispatch down instead of callbacks.

## How does it work? How does the Reducer Hook work?

Reducer Hook is used to save and update states, much like useState Hook. The reducer function is the first parameter, and the initial state is the second.

useReducer returns an array holding the current state value as well as a dispatch function to which you may submit a later-running action. There are a few differences between this design and Redux's.


## CODE EXAMPLE:

```js
import React, { useReducer } from "react";

const initialState = { count: 0 };
// The reducer function
function reducer(state, action) {
  switch (action.type) {
    case "increment":
      return { count: state.count + 1 };
    case "decrement":
      return { count: state.count - 1 };
    case "reset":
      return { count: (state.count = 0) };
    default:
      return { count: state.count };
  }
}

export default function Counter() {
  const [state, dispatch] = useReducer(reducer, initialState);
  return (
    <>
      Count: {state.count}
      <button onClick={() => dispatch({ type: "reset" })}>Reset</button>
      <button onClick={() => dispatch({ type: "decrement" })}>-</button>
      <button onClick={() => dispatch({ type: "increment" })}>+</button>
    </>
  );
}
```