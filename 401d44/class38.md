## Redux - Asynchronous Actions

### 1. How granular should your reducers be?

"Reducer functions should only depend on their state and action arguments, and should only calculate and return a new state value based on those arguments"

https://redux.js.org/style-guide/style-guide

### 2. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

Both: Pro, as his could allow a single action to update interdependent pieces of state. Con, because this could cause side-effects.

### 3. Name a strategy for preventing the above

Using good naming conventions.

### Document the following Vocabulary Terms

### store

A store holds the whole state tree of your application. The only way to change the state inside it is to dispatch an action on it.

https://redux.js.org/api/store

### combined reducers

A combined reducer is a higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.

https://redux.js.org/usage/structuring-reducers/using-combinereducers
