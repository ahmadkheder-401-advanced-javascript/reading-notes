# Express
Express is a routing and middleware web framework that has minimal functionality of its own: An Express application is essentially a series of middleware function calls.

Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.
### Order of Middleware Calls
One of the most important things about middleware in Express is the order in which they are written/included in your file; the order in which they are executed, given that the route matches also needs to be considered.


## Routing
Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing, see Basic routing.

You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function (See Using middleware for details).

These routing methods specify a callback function (sometimes called “handler functions”) called when the application receives a request to the specified route (endpoint) and HTTP method. In other words, the application “listens” for requests that match the specified route(s) and method(s), and when it detects a match, it calls the specified callback function.

In fact, the routing methods can have more than one callback function as arguments. With multiple callback functions, it is important to provide next as an argument to the callback function and then call next() within the body of the function to hand off control to the next callback.

* __SOAP:__ stands for Simple Object Access Protocol,is an acronym for Simple Object Access Protocol. It is an XML-based messaging protocol for exchanging information among computers. SOAP is an application of the XML specification.
* __ReST Verbs:__ 
  - GET :Use the HTTP GET method to obtain data.
  - POST :Use the HTTP POST method to add new rows in a dataset. See the Publisher API section for more details on how to add data.
  - PUT :Use the HTTP PUT method to modify data. Like POST, you will need authentication. Again, see the Publisher API and Authentication sections for more information.
  - DELETE :Use the HTTP DELETE method to remove data. Like POST and PUSH, you will need authentication. Again, see the Publisher API and Authentication sections for more information.


