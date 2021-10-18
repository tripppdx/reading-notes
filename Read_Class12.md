# Readings: CRUD

## Status Codes Based On REST Methods

https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/

### 1. In your own words, describe what each group of status code represents:

100’s = Informtaional
200’s = Success
300’s = Redirection
400’s = Client error
500’s = Server error

### 2. What is a status code 202?

Valid request, but processing not complete - asynchronous

### 3. What is a status code 308?

Permanent redirect - resource must be read from another URL.

### 4. What code would you use if an update didn’t return data to a client?

204 No Content

### 5. What code would you use if a resource used to exist but no longer does?

410

### 6. What is the ‘Forbidden’ status code?

403

## Build A REST API With Node.js, Express, & MongoDB - Quick

https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw

### 1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

Because when deployed we will want to use something other than our localhost and it is sensitive information.

### 2. What is middleware?

Code that runs when the sever get a request but before it gets passed to the route.

### 3. What does app.use(express.json()) do?

Allows server to accept JSON as a body instead of a POST element or a GET element (or whatever)

### 4. What does the /:id mean in a route?

It is a parameter we can access using req.parms.id which gives us access to everything passed in after the first slash.

### 5. What is the difference beween PUT and PATCH?

PATCH updates only the information that gets passed wheras PUT will update the whole record.

### 6. How do you make a defalut value in a schema?

```Javascript
subscribeDate: {
  type: Date,
  required: true,
  default: Date.now /// for example
}
```

### 7. What does a 500 error status code mean?

Error on the server, not client's fault. In the video example, our server, the database, had some kind of error which cause the transaction not to work.

### 8. What is the difference between a status 200 and a status 201?

200: general success
201: successfully created an object (more specific), bester that 201 for POST

## Things I want to know more about
