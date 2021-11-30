## Component Lifecycle / useEffect()

### 1. Why do we not need more .html pages in a multi-page React app?

Because the "pages" are build and rendered by the React router out of different components.

### 2. If we wanted a component to show up on every page, where would we put it and why?

- Inside the <BrowserRouter />, outside a <Route />

### 3. What does routing do with the components that were rendered when a new route is requested

These components are unmounted.

### 4. What does props.children contain?

" Essentially, props.children is a special prop, automatically passed to every component, that can be used to render the content included between the opening and closing tags when invoking a component. These kinds of components are identified by the official documentation as “boxes”."

https://codeburst.io/a-complete-guide-to-props-children-in-react-c315fab74e7c

### 5. How do useState() and this.setState() differ?

useState() is for functional compinents and this.setState() is for classical components. They basically do the same thing.

### Document the following Vocabulary Terms

#### State Hook

The State hook is a special React function that allows functional componenets to access and mutate state.

#### Mounting and Un-Mounting

Mounting and unmounting are React lifecycle events. Mounting refers to adding a component to the DOM. Unmounting refers to removing a component from the DOM.

https://reactjs.org/docs/state-and-lifecycle.html
