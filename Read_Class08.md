# Readings: API's

## API Design Best Practices

https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design

### 1. What does REST stand for?

Representational State Transfer

### 2. REST APIs are designed around a [__________].

RESOURCE

### 3. What is an identifer of a resource? Give an example.

An identifier is like a key that uniquely identifies the resource. An example is

```
https://adventure-works.com/orders/1
```

### 4. What are the most common HTTP verbs?

GET, POST, PUT, PATCH, DELETE

### 5. What should the URIs be based on?

URI's should be based on nouns, not verbs (the resource, not operations on the resource).

### 6. Give an example of a good URI.

```
https://adventure-works.com/orders
```

### 7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

A chatty web API is an API that requires multiple requests retrieve the desired data. This is a bad thing.

### 8. What status code does a successful GET request return?

200 (OK)

### 9. What status code does an unsuccessful GET request return?

404 (Not Found)

### 10. What status code does a successful POST request return?

201 (Created)

### 11. What status code does a successful DELETE request return?

204 (No Content)

## RegExr

https://regexr.com/

### 1. How would you match your name using RegEx?

^Harvey$

## ## Things I want to know more about

I need to learn more about regular expressions.
