# Express REST API

## Three real world use cases where you’d want to change the request with custom middleware

1. Authenticate and authorization.
2. Error Handling.
3. Parameters validation.

## The route handler is middleware?
False

## Ways can a middleware function end the process and send data to the browser

- `response.send()` .
- `response.render()` .
- `response.json()` .
- `response.redirect()` .
- `res.download()` .
- `res.end()` .
- `res.jsonp()` .
- `res.sendFile()` .
- `res.sendStatus()` .

## The point in the request lifecycle can you “inject” middleware

After client request and before response, in the middle of request and response cycle.


## What can cause express to error with “Request headers sent twice, cannot start a second response

when we are already in the Body or Finished state, but some function tried to set a header or statusCode.
> The answer from [stackoverflow.com](https://stackoverflow.com/questions/7042340/error-cant-set-headers-after-they-are-sent-to-the-client)
<br>

## ES6 classes

Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes.


Class declarations:<br>
One way to define a class is using a class declaration. To declare a class, you use the class keyword with the name of the class.<br>

Hoisting: <br>
An important difference between function declarations and class declarations is that function declarations are hoisted and class declarations are not.<br>

Class expressions: <br>
A class expression is another way to define a class. Class expressions can be named or unnamed.<br>

## Express routing

Routing refers to how an application’s endpoints (URIs) respond to client requests.

We define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests.<br> 


We can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function. <br>


The following code is an example of a very basic route:

```
var express = require('express')
var app = express()

// respond with "hello world" when a GET request is made to the homepage
app.get('/', function (req, res) {
  res.send('hello world')
})
```
Route methods:<br>
A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.

```
// GET method route
app.get('/', function (req, res) {
  res.send('GET request to the homepage')
})

// POST method route
app.post('/', function (req, res) {
  res.send('POST request to the homepage')
})
```
Route paths:<br>
Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.<br>

The characters ?, +, *, and () are subsets of their regular expression counterparts. The hyphen (-) and the dot (.) are interpreted literally by string-based paths.

Example: his route path will match acd and abcd
```
app.get('/ab?cd', function (req, res) {
  res.send('ab?cd')
})
```

We can do using express routing:

- Use express.Router() multiple times to define groups of routes.
- Apply the express.Router() to a section of our site using app.use().
- Use route middleware to process requests.
- Use route middleware to validate parameters using .param().
- Use app.route() as a shortcut to the Router to define multiple requests on a route.