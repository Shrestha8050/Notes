# Express

    Express is a minimal and flexible Node.js web application framework that provides a robust(powerful) 
    set of features for web and mobile applications.

### Software Library

    A software library is a suite of data and programming code that is used to develop software programs and applications. 
    It is designed to assist both the programmer and the programming language compiler in building and executing software.

### Software suite or Application suite

    A software suite or application suite is a collection of computer programs — usually application software or programming software — of related functionality, 
    often sharing a similar user interface and the ability to easily exchange data with each other.

### Application Framework

    An application framework is a software library that provides a fundamental structure to support the development of applications for a specific environment.
    An application framework acts as the skeletal support to build an application.

### Creates an Express application.

    The express() function is a top-level function exported by the express module.
        const express = require('express');
        const app = express();

### Response methods

    The methods on the response object (res) in the following table can send a response to the client, and terminate the request-response cycle. 
    If none of these methods are called from a route handler, the client request will be left hanging.

    Method
    - res.download() - Prompt a file to be downloaded.
    - res.end() - End the response process.
    - res.json() - Send a JSON response.
    - res.jsonp() - Send a JSON response with JSONP support.
    - res.redirect() - Redirect a request.
    - res.render() - Render a view template.
    - res.send() - Send a response of various types.
    - res.sendFile() - Send a file as an octet stream.
    - res.sendStatus() - Set the response status code and send its string representation as the response body.

# Application

    The app object conventionally denotes the Express application.
    Create it by calling the top-level express() function exported by the Express module:

        const express = require('express')
        const app = express()

        app.get('/', function (req, res) {
        res.send('hello world')
        })

        app.listen(3000)

    The app object has methods for:
        - Routing HTTP requests; see for example, app.METHOD and app.param.
        - Configuring middleware; see app.route.
        - Rendering HTML views; see app.render.
        - Registering a template engine; see app.engine.
        - It also has settings (properties) that affect how the application behaves

# Request

    The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.
        - the HTTP request is req
        - the HTTP response is res

        app.get('/user/:id', function (req, res) {
            res.send("Request To Server" + req);
            res.send('user ' + req.params.id)
        })

        OR

        app.get('/user/:id', function (request, response) {
            response.send("Request To Server" + req);
            response.send('user ' + request.params.id)
        })

# Response

    The res object represents the HTTP response that an Express app sends when it gets an HTTP request.
        - the HTTP request is req
        - the HTTP response is res

        app.get('/user/:id', function (req, res) {
            res.send('user ' + req.params.id)
        })

        OR

        app.get('/user/:id', function (request, response) {
            response.send('user ' + request.params.id)
        })

# Router

    A router object is an isolated instance of middleware and routes.
    You can think of it as a “mini-application,” capable only of performing middleware and routing functions.
    Every Express application has a built-in app router.

    A router behaves like middleware itself, so you can use it as an argument to app.use() or as the argument to another router’s use() method.

    The top-level express object has a Router() method that creates a new router object.

    Once you’ve created a router object, you can add middleware and HTTP method routes (such as get, put, post, and so on) to it just like an application. For example:

    // invoked for any requests passed to this router
    router.use(function (req, res, next) {
    // .. some logic here .. like any other middleware
        next()
    })

    // will handle any request that ends in /events
    // depends on where the router is "use()'d"
    router.get('/events', function (req, res, next) {
    // ..
    })
    You can then use a router for a particular root URL in this way separating your routes into files or even mini-apps.

    // only requests to /calendar/* will be sent to our "router"
    app.use('/calendar', router)

For More Details Information :[https://expressjs.com/en/4x/api.html]
