

## Routing
Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing, see Basic routing.

You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function (See Using middleware for details).

These routing methods specify a callback function (sometimes called “handler functions”) called when the application receives a request to the specified route (endpoint) and HTTP method. In other words, the application “listens” for requests that match the specified route(s) and method(s), and when it detects a match, it calls the specified callback function.

In fact, the routing methods can have more than one callback function as arguments. With multiple callback functions, it is important to provide next as an argument to the callback function and then call next() within the body of the function to hand off control to the next callback.



## Route methods
A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.

The following code is an example of routes that are defined for the GET and the POST methods to the root of the ap
# Use the New Router in ExpressJS 4.0
## Application Structure
```
- package.json  // set up our node packages
- server.js     // set up our app and build routes
```
## Starting Our Application
with `package.json` then install the dependencies like `express`
## Creating Our Server
We will use Express to start our application server. Since we defined `server.js` as the main file in `package.json`, that is the file that Node will use. 

```
// server.js
var express = require('express');
var app     = express();
var port    =   process.env.PORT || 8080;

// ROUTES
app.get('/sample', function(req, res) {
    res.send('this is a sample!');  
});

// we'll create our routes here

// START THE SERVER
// ==============================================
app.listen(port);
console.log('Magic happens on port ' + port);
```

## Express Router
It is a mini express application without all the bells and whistles of an express application, just the routing stuff. Let's take a look at exactly what this means. We'll go through each section of our site and use different features of the Router.
## Route Middleware router.use()
Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we'd like to do before we actually spit out information to our user.

