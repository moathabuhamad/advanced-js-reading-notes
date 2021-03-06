# ES6 Classes

## JavaScript Classes are templates for JavaScript Objects.
```
class ClassName {
  constructor() { ... }
}
```
### Example
```
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
}
```



# JavaScript Callback Functions

## What is Express middleware?
Middleware is software containing functions that execute during the request-response cycle and have access to both the request object (req) and the response object (res). Middleware is executed during the window between when a server receives a request and when it sends a response.

Express middleware includes application-level, router-level, and error handling functionality and can be built-in or from a third party. Since Express.js has limited functionality of its own, an Express app is largely comprised of multiple middleware function calls.
