# Readings: React and Forms

## React Docs - Thinking in React

https://reactjs.org/docs/thinking-in-react.html

### 1. What is the single responsibility principle and how does it apply to components?

In his book **Principles of Object Oriented Design**, Robert C. Martin defines this principle as:

> A class should have only one reason to change.

In the context of components, this means that each component should have a single purpose (e.g. displaying one piece of the JSON data model). This philosophy guides the architecture of the app and leads to a component hierarchy.

### 2. What does it mean to build a ‘static’ version of your application?

A 'static' version of an app is a version that renders the UI but is not interaactive. In this version, the only method each component should have is render(). The result is a library of components that render the data model.

### 3. Once you have a static application, what do you need to add?

At this point, it is time to make the UI interactive. You do this implementing state.

### 4. What are the three questions you can ask to determine if something is state?

According to the reading the three questions are:

> Is it passed in from a parent via props? If so, it probably isn’t state.
> Does it remain unchanged over time? If so, it probably isn’t state.
> Can you compute it based on any other state or props in your component? If so, it isn’t state.

### 5. How can you identify where state needs to live?

For a particular piece of state, you need to find the highest parent component of the components that rely on it. This is where the state needs to live. If one does not exist, one should create it.

## Higher-Order Functions

https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK

### 1. What is a “higher-order function”?

A higher-order function is a function that operates on other functions. These functions allow for abstraction which hides the low level details of the implementation and allows the programmer to think in terms of actions.

> Higher-order functions allow us to abstract over actions, not just values.

### 2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

Line 2 creates a new function

```Javascript
greaterThan10()
```

which is equal to the function

```Javascript
greaterThan(n)
```

with the parameter n predefined as 10.

### 3. Explain how either map or reduce operates, with regards to higher-order functions.

The map() method is a higher order function that abstracts the low-level details of creating a new array based on mutated values of a supplied array. It meets the definition of I higher-order function because is operates on other functions. In the case of map(), it takes a callback function as an argument.

## Things I want to know more about

> If you try to type or check the box in the current version of the example,
> you’ll see that React ignores your input.

Is this an error in the documentation, or do I not understand? Has the example been updated?
