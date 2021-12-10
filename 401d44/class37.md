## Redux - Combined Reducers

### 1. Why choose Redux instead of the Context API for global state?

Redux is superior for apps with complex state with high-frequency updates. Context will trigger a re-render on each update.

https://dev.to/ibrahima92/redux-vs-react-context-which-one-should-you-choose-2hhh

### 2. What is the purpose of a reducer?

"Reducers are functions that take the current state and an action as arguments, and return a new state result."

https://redux.js.org/tutorials/fundamentals/part-3-state-actions-reducers

### 3. What does an action contain?

An action contains a type and a payload.

### 4. Why do we need to copy the state in a reducer?

Because the reducer creates a new state object (Redux state is read-only). The copy provides a snapshot of the old state to use to populate the new object with the unmutated parts of state.

https://github.com/tur-nr/polymer-redux/issues/70

### Document the following Vocabulary Terms

### immutable state

A React/Redux state paradigm. In React, state should only be mutated through the setState() method. In Redux, mutation only occures through reducers by concatenating the old state with new state.

https://flaviocopes.com/react-immutability/

### time travel in redux

Redux uses objects to represent states, and pure functions to compute the next application state. These characteristics make Redux a predictable state container, meaning that given a specific application state and a specific action, the next state of the application is always exactly the same. That predictability makes it easy to implement time travel — the ability to move back and forth among the application’s previous states and view the results in real time.

https://developer.ibm.com/tutorials/wa-manage-state-with-redux-p4-david-geary/

### action creator

An action creator is a function that returns an action.

https://blog.isquaredsoftware.com/2016/10/idiomatic-redux-why-use-action-creators/

### reducer

In Redux, a reducer is a pure function that takes an action and the previous state of the application and returns the new state.

https://www.pluralsight.com/guides/how-to-write-redux-reducer

### dispatch

Dispatch is a function of the Redux store. You call store.dispatch to dispatch an action. This is the only way to trigger a state change.

https://react-redux.js.org/using-react-redux/connect-mapdispatch
