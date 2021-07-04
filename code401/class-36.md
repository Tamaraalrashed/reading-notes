## Application State with Redux

## Review, Research, and Discussion

### What are the advantages of storing tokens in “Cookies” vs “Local Storage”

Cookies:

- Default expiration time.
- You can access them from both the back-end (req.headers.cookie) and front-end.
 <br> 

Local Storage:

-No expiration time, you have to delete them manually (from the browser).
- Data is only accessed from the local browser. Server can't access local storage unless a request been send (POST or GET)
<br>



### Explain 3rd party cookies.

Third-party cookies are cookies that are set by a website other than the one you are currently on. For example, you can have a "Like" button on your website which will store a cookie on a visitor's computer, that cookie can later be accessed by Facebook to identify visitors and see which websites they visited. <br>

### How do pixel tags work?
A tracking pixel (also called 1x1 pixel or pixel tag) is a graphic with dimensions of 1x1 pixels that is loaded when a user visits a webpage or opens an email. ... The tracking pixel URL is the memory location on the server. When the user visits a website, the image with the tag is loaded from this server.<br>




## Terms

### cookies

A block of data that are placed on the user's website or in user's device (third-party cookies) that is used to store data about the user behavior on that website.

### Authorization

The process of giving the user different authorizes (capabilities) after he/she been authenticated.

### Access control 

is giving the user different level of access types that will allow the user to interact differently with the website based on user's role or other condition.

### Conditional rendering

rendering the UI based on different conditions, in React, it happens when we use IF component that has a condition if met the children of that component will be rendered.





## Preparation Materials


### Redux

Redux is a predictable state container for JavaScript apps.<br>

It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. On top of that, it provides a great developer experience, such as live code editing combined with a time traveling debugger. <br>

You can use Redux together with React, or with any other view library. It is tiny (2kB, including dependencies), but has a large ecosystem of addons available. <br>

### Redux Toolkit 
is the official recommended approach for writing Redux logic. It wraps around the Redux core, and contains packages and functions that we think are essential for building a Redux app. Redux Toolkit builds in our suggested best practices, simplifies most Redux tasks, prevents common mistakes, and makes it easier to write Redux applications.<br>

RTK includes utilities that help simplify many common use cases, including store setup, creating reducers and writing immutable update logic, and even creating entire "slices" of state at once.

Whether you're a brand new Redux user setting up your first project, or an experienced user who wants to simplify an existing application, Redux Toolkit can help you make your Redux code better.

`npm install @reduxjs/toolkit`

Create a React Redux App
`npx create-react-app my-app --template redux-typescript`

Redux Core

`npm install redux`

<br>

Redux is a valuable tool for organizing your state, but you should also consider whether it's appropriate for your situation. Don't use Redux just because someone said you should - take some time to understand the potential benefits and tradeoffs of using it.

***Some suggestions on when it makes sense to use Redux:***

- You have reasonable amounts of data changing over time.
- You need a single source of truth for your state.
- You find that keeping all your state in a top-level component is no longer sufficient.

