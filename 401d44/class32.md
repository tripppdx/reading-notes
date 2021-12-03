## Reading: Context API - Behaviors

### 1. When you have multiple contexts, what component type should you use (class/function) and why?

I am unable to find any documentation that asserts one component type over another. The lectures did not address the topic either. I see no advantage or disadvantage.

### 2. What are some good use cases for using the Context API for global state?

Good use cases for the Context API are when applying global settings to an app, for example, applying themes or customizing for a particular user.

### 3. How can you best test context?

"The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing)."

https://www.samdawson.dev/article/react-context-testing

### Document the following Vocabulary Terms

### context

"Context provides a way to pass data through the component tree without having to pass props down manually at every level."

https://reactjs.org/docs/context.html

### useContext()

"Accepts a context object (the value returned from React.createContext) and returns the current context value for that context. The current context value is determined by the value prop of the nearest <MyContext.Provider> above the calling component in the tree."

https://reactjs.org/docs/hooks-reference.html#usecontext

### static context

"Static content is any file that is stored in a server and is the same every time it is delivered to users."

https://www.cloudflare.com/learning/cdn/caching-static-and-dynamic-content/
