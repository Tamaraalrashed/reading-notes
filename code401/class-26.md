# Component Based UI

## Review, Research, and Discussion

### Name 5 Javascript UI Frameworks (other than React)

1. Angular.
1. Vue.
1. Ember.
1. Svelte 3.
1. Meteor. <br>

### What’s the difference between a framework and a library?

The technical difference between a framework and library lies in a term called inversion of control. When you use a library, you are in charge of the application flow. You choose when and where to call the library. When you use a framework, the framework is in charge of the flow. It provides you with a few places to plug in your code, but it calls the code you plugged in as needed.<br>




## Terms

### Rendering

Rendering is a process used in web development that turns website code into the interactive pages users see when they visit a website. The term generally refers to the use of HTML, CSS, and JavaScript codes. The process is completed by a rendering engine, the software used by a web browser to render a web page. Because of its close association with web browsers, rendering engines are commonly referred to as browser engines. <br>

### Templates

A website template is a pre designed resource that shows the structure for the comprehensive layout and display features of any website. It is provided by various suppliers to help make Web design a lot easier for designers. A website template is also known as a Web page template or page template.<br>

### State

state is how something is; its configuration, attributes, condition or information content. We will use the term component to include software and hardware "things". Virtually all components have state, from applications to operating systems to network layer.


## Preparation Materials

### React

A JavaScript library for building user interfaces.<br>

React makes it painless to create interactive UIs. Design simple views for each state in your application, and React will efficiently update and render just the right components when your data changes.<br>

Build encapsulated components that manage their own state, then compose them to make complex UIs.

Since component logic is written in JavaScript instead of templates, you can easily pass rich data through your app and keep state out of the DOM.<br>


You can develop new features in React without rewriting existing code.

React can also render on the server using Node and power mobile apps using React Native.<br>

The smallest React example looks like this:
```
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);
```
It displays a heading saying “Hello, world!” on the page.<br>

## JSX

it is a syntax extension to JavaScript.It's recommended to use with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript.

```
const element = <h1>Hello, world!</h1>;
```

## Rendering Elements

To render a React element into a root DOM node, pass both to `ReactDOM.render()`:

```
const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));
```

It displays “Hello, world” on the page.<br>


React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.<br>