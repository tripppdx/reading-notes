## Redux - Additional Topics

### 1. What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

You need to trigger an async action to fetch the data with the useEffect hook. This trigger should be placed in a higher-order component that wraps the app. Thunk middleware will be required to handle the async action, which will pass the data tpo a reducer to be placed in the store. mapStateToProps will then make the data available to the component.

https://stackoverflow.com/questions/39356517/correct-way-to-pre-load-component-data-in-reactredux

### 2. When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

The reducer exports a function instead of an action object. This function is the thunk. It will later be invoke by middleware to cause the effect.

https://medium.com/fullstack-academy/thunks-in-redux-the-basics-85e538a3fe60

### Document the following Vocabulary Terms

### middleware

Redux middleware is a snippet of code that provides a third-party extension point between dispatching an action and the moment it reaches the reducers.

https://medium.com/chingu/understanding-redux-middleware-5d8fe63aabfb

### thunk

Thunks are a functional programming technique used to delay computation.

https://medium.com/fullstack-academy/thunks-in-redux-the-basics-85e538a3fe60
