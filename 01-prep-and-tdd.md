# Content

- [JS callback functions](#javascript-callback-functions)
- [JS Promises](#javascript-promises)
- [Async/Await Function](#async-await-function-in-javascript)
- [Test-Driven Development](#test-driven-development)

# Event Loop
## The  event loop job is to look at the stack and look at the task queue. If the stack is empty, it takes the first thing on the queue and pushed it on to the stack."


# JavaScript Callback Functions

## What is a Callback Function?

In JavaScript, functions are objects. Can we pass objects to functions as parameters? Yes.
So, we can also pass functions as parameters to other functions and call them inside the outer functions.

## Why do we need Callback Functions?

JavaScript runs code sequentially in top-down order. However, there are some cases that code runs (or must run) after something else happens and also not sequentially. This is called asynchronous programming.

## What about Events?

JavaScript is an event-driven programming language. We also use callback functions for event declarations.

# JavaScript Promises

## What is a Promise?

A promise in JavaScript is similar to a promise in real life. When we make a promise in real life, it is a guarantee that we are going to do something in the future. Because promises can only be made for the future.

A promise has 2 possible outcomes: it will either be kept when the time comes, or it won’t.
This is also the same for promises in JavaScript. When we define a promise in JavaScript, it will be resolved when the time comes, or it will get rejected.

## Benefits of Promises

- Improves Code Readability.
- Better handling of asynchronous operations.
- Better flow of control definition in asynchronous logic.
- Better Error Handling.

## A Promise has four states:

fulfilled: Action related to the promise succeeded
rejected: Action related to the promise failed
pending: Promise is still pending i.e. not fulfilled or rejected yet
settled: Promise has fulfilled or rejected

## What is the difference between Callbacks and Promises?

The main difference between Callback Functions and Promises is that we attach a callback to a Promise rather than passing it. So we still use callback functions with Promises, but in a different way (chaining).

This is one of the greatest advantages of using Promises, but why?

## What is Chaining?

Callback functions have been used alone for asynchronous operations in JavaScript for many years. But in some cases, using Promises can be a better option.

# Async Await Function in JavaScript

We all know that Javascript is a Synchronous which means that it has an event loop that allows you to queue up an action that won’t take place until the loop is available sometime after the code that queued the action has finished executing. But there’s a lot of functionalities in our program which makes our code Asynchronous. One of them is the Async/Await functionality.

Async/Await is the extension of promises which we get as a support in the language. You can refer Promises in Javascript to know more about it.

## Async:

It simply allows us to write promises based code as if it was synchronous and it checks that we are not breaking the execution thread. It operates asynchronously via the event-loop. Async functions will always return a value. It makes sure that a promise is returned and if it is not returned then javascript automatically wraps it in a promise which is resolved with its value.

## Await:

Await function is used to wait for the promise. It could be used within the async block only. It makes the code wait until the promise returns a result. It only makes the async block wait.

# Test-driven development

Test-driven development (TDD) is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases. This is as opposed to software being developed first and test cases created later.
