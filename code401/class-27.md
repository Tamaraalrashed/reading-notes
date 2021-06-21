# Props and State

## Review, Research, and Discussion

### Does a deployed React application require a server?

You don't necessarily need a static server in order to run a Create React App project in production. It also works well when integrated into an existing server side app. <br>

### Why do we prefer to test a React application at the behavior rather than the unit level?

Component testing verifies the functionality of an individual part of an application. Tests are performed on each component in isolation from other components.<br>

### What does `npm run build` do?

 runs the script "build" and created a script which runs your application - let's say server.js.<br>

### Describe the actual composition / architecture of a React application

- Directory Layout.
- Component Imports.
- Function as Children.
- Render Props.
<br>

## Terms

### BDD

Behavior Driven Development, is a branch of Test Driven Development (TDD). BDD uses human-readable descriptions of software user requirements as the basis for software tests. <br>

### Acceptance Tests

 A testing technique performed to determine whether or not the software system has met the requirement specifications. The main purpose of this test is to evaluate the system's compliance with the business requirements and verify if it is has met the required criteria for delivery to end users.A.<br>

### mounting

is the phase in which our React component mounts on the DOM (i.e., is created and inserted into the DOM). This method is called just before a component mounts on the DOM or the render method is called. After this method, the component gets mounted. <br>

### build

a build is the process of converting source code files into standalone software artifact(s) that can be run on a computer, or the result of doing so.<br>



## Preparation Materials

### Handling Events

Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:<br>
- React events are named using camelCase, rather than lowercase.
- With JSX you pass a function as the event handler, rather than a string.
<br>

For example, the HTML:
```
<button onclick="activateLasers()">
  Activate Lasers
</button>
```
<br>

is slightly different in React:
```
<button onClick={activateLasers}>
  Activate Lasers
</button>
```

React events do not work exactly the same as native events. <br>

ou have to be careful about the meaning of this in JSX callbacks. In JavaScript, class methods are not bound by default. If you forget to bind this.handleClick and pass it to onClick, this will be undefined when the function is actually called.

This is not React-specific behavior; it is a part of how functions work in JavaScript. Generally, if you refer to a method without () after it, such as onClick={this.handleClick}, you should bind that method.<br>

If calling bind annoys you, there are two ways you can get around this. If you are using the experimental public class fields syntax, you can use class fields to correctly bind callbacks.<br>

### Forms

HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state. <br>

In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with `setState()`.<br>

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.<br>

### State and Lifecycle

There are three things you should know about setState().

- Do Not Modify State Directly.Instead, use setState().<br>
- State Updates May Be Asynchronous: Because this.props and this.state may be updated asynchronously, you should not rely on their values for calculating the next state, to fix it, use a second form of setState() that accepts a function rather than an object. <br>
- State Updates are Merged: when you call setState(), React merges the object you provide into the current state. <br>
  


### Components and Props

Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. <br>

Components can refer to other components in their output. This lets us use the same component abstraction for any level of detail. A button, a form, a dialog, a screen: in React apps, all those are commonly expressed as components.<br>

Props are Read-Only, all React components must act like pure functions with respect to their props. <br>


### React Testing

React Testing Library (RTL) is made of simple and complete React DOM testing utilities that encourage good testing practices.

