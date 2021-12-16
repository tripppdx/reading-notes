## React Native

### 1. Compare and Contrast Redux Toolkit with Redux “Ducks”

The "Ducks" pattern, is an organizational paradigm for Redux projects. It is recommended that an appication's files should be organized into feature based folders. "Within a given feature folder, the Redux logic for that feature should be written as a single "slice" file, preferably using the Redux Toolkit createSlice API." This contrasts with the traditional approach of seperate folders for actions and reducers.

https://github.com/erikras/ducks-modular-redux
https://redux.js.org/style-guide/style-guide

### 2. What is the principle advantage of Redux Toolkit

The principle advantage regards quality of life. It provides API's that supply logic and avoid repetition. It also save the developer from a lot of manual configuration (installing dependencies, boilerplate, etc...). It is, however, opinionated and requires you to adhere to its conventions.

https://dev.to/mmeurer00/what-is-redux-toolkit-b94

### 3. Document the following Vocabulary Terms

### redux toolkit slices

A Redux Slice is a collection of reducer logic and actions for a single feature of an app.

https://medium.com/swlh/redux-in-react-js-reducers-and-slices-bafafec781e3

### namespace

A namespace is used to uniquely identify one or more names from other similar names of different objects, groups or the namespace in general. Namespace makes it possible to distinguish objects with similar names but different origins.

https://www.techopedia.com/definition/1341/namespace
