## Hooks API

## Review, Research, and Discussion

### Why do we not need more .html pages in a multi-page React app?

Because in React we can develop SPA (Single page application) so we render the components in the same page thus we don't need to create html files.

### If we wanted a component to show up on every page, where would we put it and why?

Inside the , outside a we have to put the whole app inside the to wrap it inside React router, then the component that we want it to render on all pages should not be inside any meaning it does not need any specific path to render.

### What does props.children contain?
All the elements between the opening and closing component's tag.

## Terms

### Composition:
is the process of adding wrapping component together and creating parent and child components.

### Children / Child Components:
Component(s) between opening and closing other component (parent) tag.

### Hash Routing
When we use instead of in React Routing using react-router-dom, and it appears in the URL like this https://www.example.com/#link

### Link Routing
Is the process of creating tags with specific path to link our UI to the URL in React applications.



## Preparation Materials


### Hooks solve exactly that problem.

 Hooks let you use React features (like state) from a function — by doing a single function call. React provides a few built-in Hooks exposing the “building blocks” of React: state, lifecycle, and context.

### Hooks are a new addition in React 16.8. 
They let you use state and other React features without writing a class. Hooks don’t work inside classes. But you can use them instead of writing classes.

### A Hook is a special function that lets you “hook into” React features.
 For example, useState is a Hook that lets you add React state to function components.

What do we pass to useState as an argument? The only argument to the useState() Hook is the initial state. What does useState return? It returns a pair of values: the current state and a function that updates it. This is similar to this.state.count and this.setState in a class, except you get them in a pair.

### Hooks are JavaScript functions, but they impose two additional rules:

Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions. Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions. (There is just one other valid place to call Hooks — your own custom Hooks.

The state of each component is completely independent. Hooks are a way to reuse stateful logic, not state itself. In fact, each call to a Hook has a completely isolated state — so you can even use the same custom Hook twice in one component.

You’ve likely performed data fetching, subscriptions, or manually changing the DOM from React components before. We call these operations “side effects” (or “effects” for short) because they can affect other components and can’t be done during rendering.

The Effect Hook, useEffect, adds the ability to perform side effects from a function component. It serves the same purpose as componentDidMount, componentDidUpdate, and componentWillUnmount in React classes, but unified into a single API.<br>

What does useEffect do? By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates.<br>

Does useEffect run after every render? Yes! By default, it runs both after the first render (DidMount) and after every update (DidUpdate).<br>

Why did we return a function from our effect? This is the optional cleanup mechanism for effects. Every effect may return a function that cleans up after it.<br>

useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.<br>