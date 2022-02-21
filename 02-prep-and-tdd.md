Middleware functions are functions that have access to the request object (req), the response object (res), and the next function in the application’s request-response cycle. The next function is a function in the Express router which, when invoked, executes the middleware succeeding the current middleware.

Name 3 real world use cases where you’d want to change the request with custom middleware?
* Auth middleware
* Logging Middleware
* validateCookies

Middleware functions can perform the following tasks:
* Execute any code.
* Make changes to the request and the response objects.
* End the request-response cycle.
* Call the next middleware in the stack.

True or false: The route handler is middleware?
true A middleware is basically a function that will the receive the Request and Response objects, just like your route Handlers do.

In what ways can a middleware function end the process and send data to the browser?

If the current middleware function does not end the request-response cycle, it must call next() to pass control to the next middleware function. Otherwise, the request will be left hanging.

Types of express middleware
* Application level middleware app.use
* Router level middleware router.use
* Built-in middleware express.static,express.json,express.urlencoded
* Error handling middleware app.use(err,req,res,next)
* Thirdparty middleware bodyparser,cookieparser

At what point in the request lifecycle can you “inject” middleware?
we inject it to a module as how we want to use we implement and inject our middleware to AppModule.

if auth fails then it wont perform next route exit the middleware with error response logic.


