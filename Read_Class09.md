# Readings: FUNCTIONAL PROGRAMMING

## Functional Programming Concepts

https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa

### 1. What is functional programming?

Functional programming is a programming paradigm that is based upon the priciples of pure functions. It avoids the use of shared state and mutable data (immutability).
[reference](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)

### 2. What is a pure function and how do we know if something is a pure function?

A pure function is a function that:

a. Always returns the same result if given the same arguments (i.e. detrministic).

b. Does not cause and observable side-effects.

c. Does not rely on external state.

### 3. What are the benefits of a pure function?

The benefits of pure functions are that they make the code easire to test, maintain, and refactor.

[reference](https://medium.com/@jamesjefferyuk/javascript-what-are-pure-functions-4d4d5392d49c)

### 4. What is immutability?

Immutability means that an objects state cannot change once it is created.

### 5. What is Referential transparency?

Referential transparency means that a function always returns the same output for input parameter(s).

## Node JS Tutorial for Beginners #6 - Modules and require()

https://www.youtube.com/watch?v=xHLd36QoS4k

### 1. What is a module?

An app module is logically isolated code that perfroms a specific function. In practice, it is a single file that does a single thing. Using modules divides an app into easily maintanable pieces.

### 2. What does the word ‘require’ do?

require() is a method on the global object in node.js that essentially imports one module into another.

### 3. How do we bring another module into the file the we are working in?

```Javascript

var variable = require('pathTo/fileName') // no extension

```

### 4. What do we have to do to make a module available?

```Javascript

module.exports =  functionName;

```
