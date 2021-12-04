## Reading: <Login /> and <Auth />

### 1. Why is the Context API useful?

The big advantage pf the React Context API is that it allows data to be shared across multiple components without the need to manually pass data via props.

### 2. Can a component outside of a provider get its context?

Yes. This is the function of the useContext() hook.

### 3. What are some common use cases for using the Context API?

Common use cases for using the Context API include site themes and auth.

### 4. Describe “Context Hell”

Context hell refers to deeply nested Context Providers.

### Document the following Vocabulary Terms

### global state

Data that is shared by all components in a React app.

https://endertech.com/blog/using-reacts-context-api-for-global-state-management

### global context

In a React, context is designed to share data that can be considered global for a tree of React components.

https://reactjs.org/docs/context.html#:~:text=Context%20is%20designed%20to%20share,class%20App%20extends%20React.

### provider

The context provider provides context to its child components or other components via the useContext() hook.

https://dmitripavlutin.com/react-context-and-usecontext/

### consumer

A consumer is eithe the child of a provider or another component that uses the useContext hook to use state maintained by another component (the provider).
