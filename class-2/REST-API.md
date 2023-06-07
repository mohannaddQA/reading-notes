# Express REST API

## ES6 Classes

### Classes are a template for creating ****\_\_**** ?

Objects in JavaScript.

### Can a class declaration be hoisted ?

No, in JavaScript, class declarations are not hoisted.

### How would you describe a constructor and contextual “this” to a non-technical friend?

Imagine you want to bake a cake. You follow a recipe that tells you what ingredients to use, how to mix them, and how long to bake the cake. In programming, a constructor is like a recipe for creating objects.

A constructor is a special function that is called when you want to create a new object based on a specific blueprint (or class). It sets up the initial state and behavior of the object. It's like the first step in creating an object, where you define its characteristics and what it can do.

In programming, "this" is like a reference to the current object you're working with. It's a way to say "the object I'm currently inside". "This" helps you access the properties and methods of the object you're working on, just like you can refer to different parts of the cake when you're cooking it.

## Express Routing

### Within Express, what does routing refer to?

routing refers to the process of defining and handling different HTTP request routes in an Express application. It involves determining how the application responds to client requests for different URLs (or routes) and HTTP methods (such as GET, POST, PUT, DELETE, etc.).

### What is the difference between a route path and a route method?

The route path defines the URL pattern, and the route method determines the HTTP method used to access that route and what is done when hitting the route by this method .

### When is it appropriate to add `next` as a parameter to a route handler and what must you do if `next` has been passed to your middleware as a parameter?

It is appropriate to add `next` as a parameter to a route handler or middleware when you want to pass control to the next middleware or route handler in the chain.

If `next` has been passed as a parameter to your middleware, you must call it within your middleware to pass control to the next middleware or route handler. This ensures that the subsequent middleware or route handler is executed.

### What is an Express Router?

Express Router allows you to define routes and their handlers and methods in a modular and organized manner. It helps in structuring your application by separating routes into different files or modules.

### By what mean do we initialize `express.Router()` in an express server?

To initialize an Express Router in an Express server, you can follow these steps:

1.  Import the Express module: `const express = require('express');`
2.  Create an instance of the Express Router: `const router = express.Router();`
3.  Define routes and handlers using the router: Use `router.METHOD(PATH, HANDLER)`
4.  Mount the router on the Express app: Use `app.use(PATH, router)` to mount the router on the Express app at the specified base path.

### What do we use route middleware for?

Route middleware in Express is used for tasks such as authentication, input validation, logging, error handling, and data transformation. It allows for adding functionality to specific routes or groups of routes in a reusable manner.
