## Advanced State with Reducers

### 1. How can we ensure that an effect hook runs only once?

"If you want to run an effect and clean it up only once (on mount and unmount), you can pass an empty array ([]) as a second argument. This tells React that your effect doesn’t depend on any values from props or state, so it never needs to re-run."

https://reactjs.org/docs/hooks-effect.html

### 2. Can useState() update more than one state variable at the same time?

useState can only update one state variable at a time. However, "a functional component can have as many states as necessary by doing multiple calls of useState()."

https://dmitripavlutin.com/react-usestate-hook-guide/

### 3. Is useState() synchronous?

No, useState() is ASYCHRONOUS. You cannot update state and immediately expect to use the updated value. To get around this useEffect is used and the state we are dependent on is put in the dependence array.

https://dev.to/shareef/react-usestate-hook-is-asynchronous-1hia

### Document the following Vocabulary Terms

#### State Hook

"A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components."

https://reactjs.org/docs/hooks-state.html

#### Component Lifecycle

"Each component goes through three phases: mounting, updating and unmounting... React components are created by being mounted onto the DOM, they change or grow through updates, and finally, they can be removed or unmounted from the DOM. These three milestones are referred to as the React component lifecycle."

https://medium.com/codex/the-lifecycle-of-a-react-component-8e01332a068d
