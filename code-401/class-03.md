# Class 03 Reading Notes

## ES6 Classes

- Just as functions can be defined as function expressions and function declarations, *classes can be defined in class expressions and class declarations*

1. Classes are a template for creating _OBJECTS_.

2. Can a class declaration be hoisted?

- Class declarations behave as if they are **not** hoisted, meaning you cannot use a class before it's declared - similar to *let* and *const*

3. How would you describe a constructor and contextual “this” to a non-technical friend?

- A constructor is a way to create an object with a class. A constructor defines the criteria for the object for example if the object is a rectangle, the constructor defines the color, height and width of that object. 'this' is a keyword that refers to the object.

## Using Express Routing

> **MIDDLEWARE** functions have access to request object(req) and response object (res) and *next* middleware function --> Can execute code, make changes to req/res objects, end the req/res cycle and call the next function in the stack.

1. Within Express, what does routing refer to?

- **Routing** refers to how an application's endpoints (URI's) respond to the client requests. Routes are defined using methods such as app.get() or app.use() that handle GET and POST requests.

2. What is the difference between a route path and a route method?

- A **route method** is derived from an HTTP method (like app.get() or app.use()) and attached to an instance of the class.
  - example:
      *app.get('/', (req, res) => {
          res.send('GET request')
      })*

- A **route path**, combined with a method, defines the endpoints where the request is made. These can be strings, string patterns or regular expressions.
  
  - example:
    *app.get('/about', (req, res) => {
      res.send('about')
    })*

3. When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?

- *next* must be used if you are using more than one callback function to handle a route.

## Express Routing

1. What is an Express Router?

- Like a mini-app, provides us with routing API's like .use(), .get(), .param(), and route.

2. By what mean do we initialize express.Router() in an express server?

- We house all of the routes in the server.js file and define dependencies (express) by doing npm i express; We create a route using app.get()
  - example:
      *app.get('/about', function(req, res) {
        res.send('This is our about page')
      });*
- We need to call an instance of the Router to create the frontend routes for the app, then create routes using app.get() (like in the sample above)
  - example:
      *const router = express.Router();*
- Using the Router makes the app more modular and flexible because we can crete multiple instances of the Router

3. What do we use route middleware for?

- A way of doing something before a request is processed --> like checking if a user is authenticated, logging data for analytics, etc.

- router.use() defines the middleware --> **placement of the middleware is important!!** Javascript reads top to bottom so if a route is created before the middleware, it will happen before the middleware, the request will end and middleware will not run at that point.

## Things I want to know more about

- Creating multiple instances of a Router - would we only do this if our app was modularized into separate components?

- Using the next parameter in the middleware vs in a route handler
