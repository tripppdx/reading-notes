## useState() Hook

### 1. How does React differ from vanilla JS/HTML/CSS?

The biggest difference between React and vanilla JS/HTML/CSS is that React automatically updates the UI based on state changes within components rather than requiring manual manipulation of the DOM. Another big difference is the fact that React stores data in regular variables, not the DOM itself. In addition, the React UI is created dynamically in the client by JavaScript, not on the server by HTML.

https://www.framer.com/blog/posts/react-vs-vanilla-js/

### 2. What is the primary difference between a function component and a class component?

It used to be that the primary difference bewteen a function component and a class component was that a class component was that a class component provided developers with access to state methods and lifecycle methods. This changed with the advent of Hooks in React 16.8.

https://flatlogic.com/blog/functional-components-vs-class-components-in-react-js/
https://javascript.plainenglish.io/the-definitive-guide-to-react-class-vs-functional-components-481b1157ed08

### Document the following Vocabulary Terms

### Functional Components

A functional component consists of a JavaScript function that takes in props as an argument and returns JSX. It accesses state and lifecycle events through the use of Hooks.

https://www.robinwieruch.de/react-function-component/#react-function-component-example

### Children / Child Components

Child components are components that are nested within higher-order parent coomponents. Data is only passed one way downward from parent to child.

https://medium.com/@lizdenhup/understanding-unidirectional-data-flow-in-react-3e3524c09d8e
