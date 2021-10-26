# Readings: Authentication

## 1. Explain what a “Singleton” is (in Computer Science terms)

In software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system.

https://en.wikipedia.org/wiki/Singleton_pattern

## 2. Explain how the Singleton pattern can be used with Node modules, specifically with classes

https://medium.com/swlh/node-js-and-singleton-pattern-7b08d11c726a

## 3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

I would build it using an error-first callback approach. In my routes, I would declare my middleware route handling fuctiions seperately in a router and set them as callbacks for the responses:

```javascript
app.use(middleware);
```

https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction

## Vocabulary

### Router Middleware

Code that comes in the middle of the request and the response.

### Dynamic Module Loading

https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction

https://en.wikipedia.org/wiki/Dynamic_loading#:~:text=Dynamic%20loading%20is%20a%20mechanism,unload%20the%20library%20from%20memory.

### Singleton Pattern

In software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system.

https://en.wikipedia.org/wiki/Singleton_pattern

### CRUD -> REST Method Matches

```plaintext
Create = PUT with a new URI
         POST to a base URI returning a newly created URI
Read   = GET
Update = PUT with an existing URI
Delete = DELETE
```

https://stackoverflow.com/questions/6203231/which-http-methods-match-up-to-which-crud-methods

### Mock Testing

Creating a fake version of an external or internal service that can stand in for the real one

https://circleci.com/blog/how-to-test-software-part-i-mocking-stubbing-and-contract-testing/
