## Redux - Asynchronous Actions

## Redux Async Data Flow
Just like with a normal action, we first need to handle a user event in the application, such as a click on a button. Then, we call dispatch(), and pass in something, whether it be a plain action object, a function, or some other value that a middleware can look for. Once that dispatched value reaches a middleware, it can make an async call, and then dispatch a real action object when the async call completes. When we add async logic to a Redux app, we add an extra step where middleware can run logic like AJAX requests, then dispatch actions.



## Redux Middleware and Side Effects​
It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Earlier, we said that Redux reducers must never contain «side effects». However, any real app will need to do these kinds of things somewhere. Redux middleware were designed to enable writing logic that has side effects.
Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store's dispatch method, which is then used to dispatch regular synchronous actions inside the function's body once the asynchronous operations have been completed.

## Extra:
Which is better Saga or thunk?
Saga works like a separate thread or a background process that is solely responsible for making your side effects or API calls unlike redux-thunk, which uses callbacks which may lead to situations like 'callback hell' in some cases. However, with the async/await system, this problem can be minimized in redux-thunk
