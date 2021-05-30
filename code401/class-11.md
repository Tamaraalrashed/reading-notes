# Event Driven Applications


# Review, Research, and Discussion

### Why is access control important?

Access controls limit access to information and information processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorization, unlawfully and the risk of a data breach.

### Describe an application that would need access control.

Any application needs to be updated to its database will need access control for make the admin to write, update or delete, but for the user will be a limited access maybe just read or sometimes write(news applications).

### What is a role used for?

User Roles are permission sets that control access to areas and features within the Professional Archive Platform. Each User account requires a Role assignment.

### Why is role based access control more scalable than discretionary or mandatory access control?

role based access control is considered to strike a good balance between security and manageability.


## Vocabulary Terms

### Authorization 
Authorization is the function of specifying access rights/privileges to resources, which is related to general information security and computer security, and to access control in particular.

### Role Based Access Control
is an approach to restricting system access to authorized users. It is used by the majority of enterprises with more than 500 employees, and can implement mandatory access control (MAC) or discretionary access control (DAC).

### Capabilities
 A capability is a communicable, unforgettable token of authority. It refers to a value that references an object along with an associated set of access rights. A user program on a capability-based operating system must use a capability to access an object.

 ## Preparation Materials

 ### Event-Driven Programming in Node.js

 Every time you interact with a webpage through it’s user interface, an event is happening. When you click a button a click event is triggered. When you press a key a keydown event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way.

- Event-Driven Programming makes use of the following concepts:

- An Event Handler is a callback function that will be called when an event is triggered.
A Main Loop listens for event triggers and calls the associated event handler for that event.

### EventEmitter
Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. Of course, creating our own version of EventEmitter wouldn’t be much of a challenge, and in fact there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.<br>

We access the EventEmitter class through the `events `module. Once imported we’ll need to create a new object from the class to start using it.

```const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter;
```

#### Much of the Node.js core API is built around an idiomatic asynchronous event-driven architecture in which certain kinds of objects (called "emitters") emit named events that cause Function objects ("listeners") to be called.
<br>

All objects that emit events are instances of the `EventEmitter` class. These objects expose an `eventEmitter.on()` function that allows one or more functions to be attached to named events emitted by the object. Typically, event names are camel-cased strings but any valid JavaScript property key can be used.<br>

When the EventEmitter object emits an event, all of the functions attached to that specific event are called synchronously. Any values returned by the called listeners are ignored and discarded. <br>

Example:
```
const EventEmitter = require('events');

class MyEmitter extends EventEmitter {}

const myEmitter = new MyEmitter();
myEmitter.on('event', () => {
  console.log('an event occurred!');
});
myEmitter.emit('event');
```