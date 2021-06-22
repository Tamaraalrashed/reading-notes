# Component Composition

## Review, Research, and Discussion

### Can a parent component access the state of a child component?

In React we can access the child's state using Refs. we will assign a Refs for the child component in the parent component. then using Refs we can access the child's state. <br>

### What can be passed along in a prop variable?

State or props.<br>

### How can a child component “know” the state of another component?

Reading props.<br>


## Terms

### Component props

Props are arguments passed into React components. Props are passed to components via HTML attributes. <br>

### Component state

The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.<br>

### Application state

The state is just a fancy term for a JavaScript data structure. If a user changes state by interacting with your application, the UI may look completely different afterwards, because it's represented by this new state rather than the old state. Make a state variable responsible for one concern to use efficiently. <br>


## Preparation Materials

### The Component Lifecycle

it details the life of a component. Like us, components are born, do some things during their time here on earth, and then they die 
<br>

A component can only be in one stage at a time. It starts with mounting and moves onto updating. It stays updating perpetually until it gets removed from the virtual DOM. Then it goes into the unmounting phase and gets removed from the DOM.<br>


### Mounting
Since class-based components are classes, hence the name, the first method that runs is the constructor method. Typically, the constructor is where you would initialize component state.

Next, the component runs the getDerivedStateFromProps.<br>

Now we come to the render method which returns your JSX. Now React “mounts” onto the DOM.

Lastly, the componentDidMount method runs. Here is where you would do any asynchronous calls to databases or directly manipulate the DOM if you need. Just like that, our component is born.

## Updating
This phase is triggered every time state or props change. Like in mounting, getDerivedStateFromProps is called (but no constructor this time!).<br>

Next shouldComponentUpdate runs. Here you can compare old props/state with the new set of props/state. You can determine if your component should re-render or not by returning true or false. This can make your web app more efficient by cutting down on extra re-renders. If shouldComponentUpdate returns false, this update cycle ends.<br>

## Unmounting

Our component lived a good life, but all good things must come to an end. The unmounting phase is that last stage of the component lifecycle. When you remove a component from the DOM, React runs componentWillUnmount right before it gets removed. You should use this method to clean up any open connections such as WebSockets or intervals.<br>

## Composition vs Inheritance

Some components don’t know their children ahead of time. This is especially common for components like Sidebar or Dialog that represent generic “boxes”. <br>

It's recommended that such components use the special children prop to pass children elements directly into their output.<br>

```
function FancyBorder(props) {
  return (
    <div className={'FancyBorder FancyBorder-' + props.color}>
      {props.children}
    </div>
  );
}
```
This lets other components pass arbitrary children to them by nesting the JSX:

```
function WelcomeDialog() {
  return (
    <FancyBorder color="blue">
      <h1 className="Dialog-title">
        Welcome
      </h1>
      <p className="Dialog-message">
        Thank you for visiting our spacecraft!
      </p>
    </FancyBorder>
  );
}
```

Anything inside the `<FancyBorder>` JSX tag gets passed into the FancyBorder component as a children prop. Since FancyBorder renders {props.children} inside a `<div>`, the passed elements appear in the final output.
