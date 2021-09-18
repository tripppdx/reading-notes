# Readings: State and Props

## Reading

React: Component Lifecycle Events
https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093
by Joshua Blankenship

### 1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

The 'render' happens before the 'componentDidMount'. These both occur during the mounting phase of the component lifecycle. The lifecycle events that occur in this phase are (in order): 'constructor', 'getDerivedStateFromProps', 'render', and 'componentDidMount.'

### 2. What is the very first thing to happen in the lifecycle of React?

The very first thing to happen in the lifecycle of React is Mounting. There are three phases of the component lifecycle. These phases are (in order): 'Mounting', 'Updating', and 'Unmounting'.

### 3. Put the following things in the order that they happen: 'componentDidMount', 'render', 'constructor', 'componentWillUnmount', 'React Updates'

These React lifecycle events happen in the following order:

'constructor'
'render'
'componentDidMount'
'React Updates'
'componentWillUnmount'

'constructor' and 'render' occur during the Mounting phase. 'React Updates' is assumed to refer to the Updating phase of the lifecycle. (Note: 1. 'render' or 're-rendering' also occurs during the Updating phase after every state change. 2. render() is the only method required in a class component).

### 4. What does componentDidMount do?

The 'componentDidMount' method is invoked immediately after a component is mounted at the end of the Mounting phase of the React lifecycle. Each lifecycle phase consists of three sub-phases that occur in the following order:

"Render phase"
"Pre-commmit phase"
"Commit phase"

'componentDidMount' occurs at the end of the commit sub-phase of the Mounting phase of the component's lifecycle. During the "commit phase", the component can work with the DOM, run side effects, and schedule updates. As a result, this method is where network requests and DOM initialization should occur.

## Video

React State Vs Props
https://www.youtube.com/watch?v=IYvD9oBCuJI

### 1. What types of things can you pass in the props?

Props can be considered to be like arguments to a function. They are the initial parameters that get passed into a React component when it is initialized and rendered. Examples include an initial counter value, a title, or a subtitle.

### 2. What is the big difference between props and state?

The big difference between props and state relates to to where each is handled and updated. Props are parameters that get passed into a component and are handled externally (e.g. by a parent). State is handled and updated internally by the component. For example, the initial value of a counter could be passed into a component by a prop. Updates to the counter state would be handled by the component itself.

### 3. When do we re-render our application?

We re-render our application in response to state changes. These state changes can happen both external and internal to individual components. In the case of external state changes, updated props get passed in that result in re-rendering. State changes internal to the component result in the component re-rendering itself

###4. What are some examples of things that we could store in state?
An important example of something that we can be stored in state is user input. For instance, anything inside a form rendered by the component would be stored in state.

## Things I want to know more about

What triggers a component to re-render when there are external changes to the props (e.g. as result of a state change in the parent component).
