# Readings: Passing Functions as Props

## Reading

## React Docs - lists and keys

https://reactjs.org/docs/lists-and-keys.html

### 1.What does .map() return?

.map() returns a new array

### 2. If I want to loop through an array and display each value in JSX, how do I do that in React?

You would need to iterate over the array and transform it into a new array of renderable JSX fragments. The easiest way of achieving this is to use the map() method. For example, this new array could consist of <li> elements that can then be passed to the render() method as an expression inside a <ul> element.

### 3. Each list item needs a unique \_\_\_\_.

KEY - note that this key need only be unique among siblings (not required to be globally unique)

### 4. What is the purpose of a key?

A key is a JSX element string attribute that serves to uniquely identify each element contained in a list. This unique identifier allows React to track each individual element throughout its lifecycle. Keys should be added to each item of the new JSX element array returned by the .map() method. This provides a stable identity.

## The Spread Operator

https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab

### 1. What is the spread operator?

The spread operator is JavaScript syntax that EXPANDS or SPREADS an iterable object (such as an array) into seperate arguments.

### 2. List 4 things that the spread operator can do.

The spread operator can be used to:

- combine arrays
- add items to an array
- combine objects
- add state in React

### 3. Give an example of using the spread operator to combine two arrays.

```javascript
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const newArr = [...arr1, ...arr2]; // [1, 2, 3, 4, 5, 6]
```

### 4. Give an example of using the spread operator to add a new item to an array.

```javascript
const arr2 = [4, 5, 6];
const newArr = [1, 2, 3, ...arr2]; // [1, 2, 3, 4, 5, 6]
```

### 5. Give an example of using the spread operator to combine two objects into one.

```javascript
const obj1 = { firstName: "Foo" };
const obj2 = { lastName: "Bar" };
const newObj = { ...obj1, ...obj2 }; // {firstName: 'Foo', lastName: 'Bar'}
```

## Videos

https://www.youtube.com/watch?v=c05OL7XbwXU

### 1. In the video, what is the first step that the developer does to pass functions between components?

The first step the developer does to pass a function between components is to the create the function in the component where the state is to be changed. In this case, it is the parent of the Person component and is defined in App.js.

### 2. In your own words, what does the increment function do?

The increment function loops through the people array in the parent component and increments the count property corresponding to the child component whose buttton is clicked.

### 3. How can you pass a method from a parent component into a child component?

You can pass a method from a parent component into a child component as a prop.

### 4. How does the child component invoke a method that was passed to it from a parent component?

The child component invokes a method (methodName) passed to it from a parent component by calling it like:

this.props.methodName(this.props.parameter)

## Bookmark

https://reactjs.org/tutorial/tutorial.html
https://reactjs.org/docs/lifting-state-up.html

## Things I want to know more about

1. Best practices for generating keys.
2. Rendering fragments that are not <li> elements.
3. More on passing functions between components.
