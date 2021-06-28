## Custom Hooks

## Review, Research, and Discussion

### What does a component’s lifecycle refer to?

Every React Component has a lifecycle of its own, lifecycle of a component can be defined as the series of methods that are invoked in different stages of the component’s existence. 

### Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect?

Because it will prevent recreation of a function.

### Why are functional components preferred over class components?
Less code, easy to read and test.

### What is wrong with the following code?
Using useEffect inside a loop.

## Terms

### State hook
 A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.

### Effect hook
The Effect Hook, useEffect , adds the ability to perform side effects from a function component. It serves the same purpose as componentDidMount , componentDidUpdate , and componentWillUnmount in React classes, but unified into a single API.

### Reducer hook

The useReducer is a hook I use sometimes to manage the state of the application. … It acts as an alternate hook to the useState hook to manage complex state in your application. The useReducer hook uses the same concept as the reducers in Redux. It is basically a pure function, with no side-effects.
is the process of adding wrapping component together and creating parent and child components.



## Preparation Materials


### Custom Hooks

- Never call Hooks from inside a loop, condition or nested function Hooks should sit at the top-level of your component Only call Hooks from React functional components Never call a Hook from a regular function Hooks can call other Hooks. <br>

- Context allows this sharing of values between components without having to explicitly pass a prop through every level of the tree.  <br>

### We can use Async/Await in our functional component when we are making requests from another API.

- We cannot use 'async' keyword with 'useEffect' callback method. It will result in race conditions.

- useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.

`const [state, dispatch] = useReducer(reducer, initialArg, init);`

- We can also create the initial state lazily. To do this, you can pass an init function as the third argument. The initial state will be set to init(initialArg).

- Pass an inline callback and an array of dependencies. useCallback will return a memoized version of the callback that only changes if one of the dependencies has changed.

`useCallback(fn, deps) is equivalent to useMemo(() => fn, deps) `.

- `useRef` returns a mutable ref object whose .current property is initialized to the passed argument (initialValue).
  
   `const refContainer = useRef(initialValue);`

Essentially, useRef is like a “box” that can hold a mutable value in its current property.

- When we want to share logic between two JavaScript functions, we extract it to a third function. Both components and Hooks are functions, so this works for them too!

  A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks.

