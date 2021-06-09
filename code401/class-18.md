# API, Dynamo and Lambda

## Review, Research, and Discussion

### What are serverless functions?

 Serverless functions are single-purpose, programmatic functions that are hosted on managed infrastructure. These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies. The engineering teams within those companies ensure that the serverless functions have near-perfect uptime, redundant instances around the world, and scale to any incoming network request volume.
 <br>

### If you were to create a system that emulated Lambda functions, how would you do it?

To create a Lambda function with the console:

1. Open the Functions page on the Lambda console.

1. Choose Create function.

1. Under Basic information, do the following:

   1. For Function name, enter my-function.

   1. For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell,C#) Go, Java, Node.js, Python, and Ruby.

1. Choose Create function.

Lambda creates a Node.js function and an execution role that grants the function permission to upload logs. The Lambda function assumes the execution role when you invoke your function, and uses the execution role to create credentials for the AWS SDK and to read data from event sources. <br>

### Describe how a CDN works

 The goal of the CDN is to reduce latency – the delay between submitting a request for a web page and the web page fully loading on your device – by reducing the physical distance that the request has to travel.<br>




## Terms

### Serverless Functions

It is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.<br>

### Cloud Storage

 a model of computer data storage in which the digital data is stored in logical pools, said to be on "the cloud". The physical storage spans multiple servers (sometimes in multiple locations), and the physical environment is typically owned and managed by a hosting company. These cloud storage providers are responsible for keeping the data available and accessible, and the physical environment secured, protected, and running. People and organizations buy or lease storage capacity from the providers to store user, organization, or application data.<br>

### CDN

A content delivery network (CDN) refers to a geographically distributed group of servers which work together to provide fast delivery of Internet content. <br>



## Preparation Materials


### - Amazon API Gateway

Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

Many Serverless applications use Amazon API Gateway, which conveniently replaces the API servers with a managed serverless solution. <br>

API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation. <br>

API Gateway integrates with many other AWS services like AWS Lambda, AWS SNS, AWS IAM, and Cognito Identity Pools. These integrations allow for fully managed authentication and authorization layers, as well as detailed metrics and tracing for API requests. <br>


### - DynamoDB

DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:

- reliable performance even as it scales;
- a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
- a small, simple API allowing for simple key-value access as well as more advanced query patterns.<br>

#### Benefits:
- Performance at scale.
- No servers to manage.
- Enterprise ready.

#### Applications:
  - Serverless Web Apps.
  - Mobile Backends.
  - Microservices.






