## Reading: Context API

### 1. Describe use cases useState() vs useReducer()

"useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks."

https://reactjs.org/docs/hooks-reference.html

### 2. Why do custom hooks need the use prefix?

Custom hooks should have the use prefix so that the developer can easily tell that the function is a hook and that the rules of Hooks apply to it. It is not required semantically.

https://reactjs.org/docs/hooks-custom.html

### 3. What do custom hooks usually do?

Custom hooks afre useful to extract component logic into usable functions.

https://reactjs.org/docs/hooks-custom.html

### 4. Using any list of custom hooks, research and name one that you think will be useful in your applications

The useFormState React hook seems particularly useful due to the fact that both React labs so far use forms and the are ubiquitous on the web.

https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d

### 5. Describe how a hook that fetches API data might work

We sort of did this in RESTy. We could have made a hook that takes advantage of useEffect which makes an API call whenver a relevant piece of state changes.

### Document the following Vocabulary Terms

### reducer

Reducers are functions that take the current state and an action as arguments, and return a new state result.

https://redux.js.org/tutorials/fundamentals/part-3-state-actions-reducers
