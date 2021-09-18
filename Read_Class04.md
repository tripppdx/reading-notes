# Readings: React and Forms

## React Docs - Forms

https://reactjs.org/docs/forms.html

### 1. What is a ‘Controlled Component’?

A 'Controlled Component' is an HTML form element (such as an <input>) whose value is controlled by React. In this paradigm, the The React component that renders the form also controls the elements value. Rather than the form element maintaining its own state based on user input, its attributes are controlled by React.

### 2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

We should update the state with the users responses as soon as they enter them. In this fashion, the controlled component allows React to sense changes and update state. As a result, React is the "single source of truth."

### 3. How do we target what the user is entering if we have an event handler on an input field?

We target what the user is entering by using a prop to attach an event handler that updates state to the onChange attribute. As a result, React state will be updated on every user interaction (e.g. on every keystroke).

## The Conditional (Ternary) Operator Explained

https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff

### 1. Why would we use a ternary operator?

We would use a ternary operator in in place of an if statement to simplify expression the expression and improve readability.

### 2. Rewrite the following statement using a ternary statement:

```Javascript

  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }

x === y ?  console.log(true) : console.log(false);

```

## Things I want to know more about

How React keeps track of state under the hood.
