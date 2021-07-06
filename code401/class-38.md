# Redux - Asynchronous Actions

## Review, Research, and Discussion

### How granular should your reducers be?

They should be pure functions with no side-effects
 <br> 




### Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

is a pro thing because it will help in letting reducers communicate with each other in kind a way. <br>



### Name a strategy for preventing the above

using different actions.<br>


## Terms

### Store
 the place where the initial state, reducer and actions are placed in one place in Redux.

### combined reducers:
 the process of using more than one reducer in our store.





## Preparation Materials


### Redux Thunk
By default, Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects. Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers.<br>

There are two very popular middleware libraries that allow for side effects and asynchronous actions: Redux Thunk and Redux Saga. <br>

Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation.

Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed. <br>

#### *Adding redux-thunk*

 `npm install redux-thunk@2.3.0`


 Redux middleware were designed to enable writing logic that has side effects.<br>
"Side effects" are code that changes state/behavior outside a function, like AJAX calls, modifying function arguments, or generating random values, and Middleware add an extra step to the standard Redux data flow. <br>
Middleware can intercept other values passed to dispatch
Middleware have access to dispatch and getState, so they can dispatch more actions as part of async logic.<br>
The Redux "Thunk" middleware lets us pass functions to dispatch. <br>
"Thunk" functions let us write async logic ahead of time, without knowing what Redux store is being used
A Redux thunk function receives dispatch and getState as arguments, and can dispatch actions like "this data was received from an API response". <br>




