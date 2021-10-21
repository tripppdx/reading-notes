# Readings: Express REST API

### Name 3 real world use cases where you’d want to change the request with custom middleware.

1. User authentication
2. Parse specific info from request
3. Error handling

### True or false: The route handler is middleware?

FALSE

### In what ways can a middleware function end the process and send data to the browser?

res.redirect()
res.end()

### At what point in the request lifecycle can you “inject” middleware?

Immediately following the receipt of the request.

### What can cause express to error with “Request headers sent twice, cannot start a second response”

Duplicate responses.

### Document the following Vocabulary Terms

#### Middleware

Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle

https://expressjs.com/en/guide/using-middleware.html

#### Request Object

The Request object retrieves the values that the client browser passed to the server during an HTTP request.

https://docs.microsoft.com/en-us/previous-versions/iis/6.0-sdk/ms524948(v=vs.90)

#### Response Object

The Response object to send output to the client.

https://docs.microsoft.com/en-us/previous-versions/iis/6.0-sdk/ms525405(v=vs.90)

#### Application Middleware

Application level middleware are bound to an instance of express, using app.use() and app.VERB().

https://stackoverflow.com/questions/29457008/whats-the-difference-between-application-and-router-level-middleware-when-rou

#### Routing Middleware

Router level middleware work just like application level middleware except they are bound to an instance of express.Router().

https://stackoverflow.com/questions/29457008/whats-the-difference-between-application-and-router-level-middleware-when-rou

#### Test Driven Development

“Test-driven development” refers to a style of programming in which three activities are tightly interwoven: coding, testing (in the form of writing unit tests) and design (in the form of refactoring).

https://www.agilealliance.org/glossary/tdd

#### Behavioral Testing

Behavioural Testing is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.

https://www.tutorialspoint.com/software_testing_dictionary/behaviour_testing.htm
