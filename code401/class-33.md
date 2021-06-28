## Context API

## Review, Research, and Discussion

### Describe use cases for useMemo() and useReducer()?

useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.<br>

 useMemo() Returns a memoized value.<br>


### Why do custom hooks need the use prefix?

it's a naming convention to all custom hooks + because both components and hooks are JS function so it's a way to differentiate between them.<br>

### What do custom hooks usually do?
Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.<br>

### Using any list of custom hooks, research and name one that you think will be useful in your applications 

react-fetch-hook.

### Describe how a hook that fetches API data might work?

It may have async functions that await to fetching data from API, it may use `fetch` , `axios` or `superagent` , then it handles the received data maybe be sending them to a state and use this state inside JSX.


## Terms

### Reducer
The useReducer is a hook I use sometimes to manage the state of the application. … It acts as an alternate hook to the useState hook to manage complex state in your application. The useReducer hook uses the same concept as the reducers in Redux. It is basically a pure function, with no side-effects.
is the process of adding wrapping component together and creating parent and child components.




## Preparation Materials


### Context

- Context provides a way to pass data through the component tree without having to pass props down manually at every level.


- Context allows this sharing of values between components without having to explicitly pass a prop through every level of the tree.  <br>

- Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.
  
  ### API

- `React.createContext`
- `Context.Provider`
- `Class.contextType`
- `Context.Consumer`
- `Context.displayName`.

