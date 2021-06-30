## `<Login />` and `<Auth />`

## Review, Research, and Discussion

### Why is the Context API useful?

The React Context API is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux.<br>



### Can a component outside of a provider get its context?

No it can not. <br>

### What are some common use cases for using the Context API?
Some sample use cases where the Context API proves helpful are: Theming — Pass down app theme. i18n — Pass down translation messages. Authentication — Pass down current authenticated user.<br>

### Describe “Context Hell”
the React Context hell is the nasty code you get taking advantage of the React Context API (Providers inside Providers ...). 





## Terms

### global state

State of Component that is used by other Component.

### global context
Context Provider that is used for the whole App and wrap all the components.

### provider
Context API that is considered as (parent) and share it's state to all its children.

### consumer
Context API that is considered as (Child) and have access to whatever the parent is sharing.





## Preparation Materials


### ROLE-BASED ACCESS CONTROL (RBAC)

Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network. <br>

Employees are only allowed to access the information necessary to effectively perform their job duties. Access can be based on several factors, such as authority, responsibility, and job competency. In addition, access to computer resources can be limited to specific tasks such as the ability to view, create, or modify a file.<br>

As a result, lower-level employees usually do not have access to sensitive data if they do not need it to fulfill their responsibilities. This is especially helpful if you have many employees and use third-parties and contractors that make it difficult to closely monitor network access. Using RBAC will help in securing your company’s sensitive data and important applications. <br>

Some of the designations in an RBAC tool can include: <br>

- Management role scope – it limits what objects the role group is allowed to manage.
- Management role group – you can add and remove members.
- Management role – these are the types of tasks that can be performed by a specific role group.
- Management role assignment – this links a role to a role group.

### BENEFITS OF RBAC
- Reducing administrative work and IT support.
- Maximizing operational efficiency.
- Improving compliance. 
- 

