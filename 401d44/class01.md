# Node Ecosystem, TDD, CI/CD

### 1. Describe (in plain English) what Array.map() does.

Array.map() is a Javascript array method that iterates over an array, executes a supplied callback function on each element, and returns a new array containing the results. It does not mutate the original array. Its signature is:

```javascript
arr.map(callbackFn(element, index, array), thisArg);
```

source: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map

### 2. Describe (in plain English) what Array.reduce() does.

Array.reduce() is a JavaScript array method that returns a single value (of any type) by executing a supplied callback function on each element of an array. The callback function is often referred to as the reducer and the returned value as the accumulator. Its signature is:

```javascript
arr.reduce(
  callbackFn(accumulator, currentValue, index, sourceArray),
  initialValue
);
```

source: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce

### 3. Provide code snippets showing how to use superagent() to fetch data from a URL and log the result:

#### With normal Promise .then() syntax

```javascript
superagent.get("/api/pet").then(console.log).catch(console.error);
```

#### Again with async / await syntax

```javascript
async () => {
  try {
    const res = await superagent.get("/api/pet");
    console.log(res);
  } catch (err) {
    console.error(err);
  }
};
```

source: https://github.com/visionmedia/superagent, https://www.npmjs.com/package/superagent

### 4. Explain promises as though you were mentoring a Code 301 level student

> "A promise is an object that may produce a single value some time in the future"
>
> -- Eric Elliot

A promise can exist in any of three states:

1. Fulfilled
2. Rejected
3. Pending

The value produced can be either the resolved value or an error code.

source: https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-promise-27fc71e77261

### 5. Are all callback functions considered to be Asynchronous? Why or Why Not?

No, callback functions can be both synchronous and asynchronous. A synchronous callback function is executed during the execution of the function that uses it and is, therefore, blocking. An asynchronous callback function is executed after the execution of the function using it and is non-blocking.

source: https://dmitripavlutin.com/javascript-callback/
