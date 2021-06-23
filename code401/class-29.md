# Routing

## Review, Research, and Discussion

### Do child components have direct access to props/state from the parent?

There is no way to pass props from a child component to a parent component. However, we can always pass around functions from the parent to child component. The child component can then make use of these functions. The function can then update the state in a parent component, as we saw above. <br>

### When a component “wraps” another component, how does the child component’s output get rendered?

It’s rendered when there is an update to state.<br>

### Can a component, such as `<Content />` , which is a child also be used as a standalone component elsewhere in the application?

Yes, we can. <br>

### What trick can a parent use to share all props with it’s children?

You can do so with the spread operator `{...props}`


## Terms

### props.children

what this.props.children does is that it is used to display whatever you include between the opening and closing tags when invoking a component. <br>

### Composition

 React Composition is a development pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop.<br>


## Preparation Materials

### React Router 

 React Router v4 is a pure React rewrite of the popular React package. Previous versions of React Router used configuration disguised as pseudo-components and could be difficult to understand. With v4, everything is “just components”.

 #### Installation

 React Router has been broken into three packages: react-router, react-router-dom, and react-router-native.

#### The Router

When starting a new project, you need to determine which type of router to use. For browser based projects, there are <BrowserRouter> and <HashRouter> components. <br>

The <BrowserRouter> should be used when you have a server that will handle dynamic requests (knows how to respond to any possible URI), while the <HashRouter> should be used for static websites (where the server can only respond to requests for files that it knows about).

Usually it is preferable to use a <BrowserRouter>, but if your website will be hosted on a server that only serves static files, then the <HashRouter> is a good solution.

#### History
Each router creates a history object, which it uses to keep track of the current location 1 and re-render the website whenever that changes. The other components provided by React Router rely on having that history object available through React’s context, so they must be rendered as descendants of a router component. A React Router component that does not have a router as one of its ancestors will fail to work.

#### Rendering a <Router>

```
import { BrowserRouter } from 'react-router-dom';

ReactDOM.render((
  <BrowserRouter>
    <App />
  </BrowserRouter>
), document.getElementById('root'));
```

#### Routes

The `<Route>` component is the main building block of React Router. Anywhere that you want to only render content based on the location’s pathname, you should use a `<Route>` element.

