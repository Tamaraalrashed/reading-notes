# AWS: Events

## Review, Research, and Discussion

### Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server

Express Gateway is an open source API Gateway written in Node.js and built on top of Express.js and Express Middleware,Amazon API Gateway is a closed-source software-as-a-service (SaaS) product written in Node.js available only on AWS. Amazon API Gateway can be considered a backplane in the cloud to connect AWS services and other public or private websites, but both of them have the same concept to do their job. <br>

### List the AWS Database offerings and talk about the pros and cons of each

1. Dynamoose .<br>
2. Amazon RDS:
   - Pros:Automated Patching,Automated Backups, Encryption at rest and in-transit.
   - Cons:Patching forces a downtime, No scale-out for write workloads,No root access to the server.


### What’s the difference between a FIFO and a standard queue?

Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue. FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue. <br>

### How can the server be assured a message was properly received?

A Message Authentication Code (MAC) is a tag attached to a message to ensure the integrity and authenticity of the message. It is derived by applying a MAC algorithm to a message in combination with a secret key. <br>


## Terms

### Serverless API 

Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider. <br>

### Triggers

Triggers are external events or circumstances that may produce very uncomfortable emotional or psychiatric symptoms, such as anxiety, panic, discouragement, despair, or negative self-talk.<br>

### Dynamo vs Mongo

DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas. ... DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents. DynamoDB supports limited data types and smaller item sizes; MongoDB supports more data types and has fewer size restrictions. <br>

### Dynamoose vs Mongoose

Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familiar.<br>



## Preparation Materials

### SNS

Amazon Simple Notification Service (Amazon SNS) is a web service that enables you to build distributed web-enabled applications. Applications can use Amazon SNS to easily push real-time notification messages to interested subscribers over multiple delivery protocols. For more information about this product see the Amazon SNS product page. For detailed information about Amazon SNS features and their associated API calls.<br>


*Constructor Summary* <br>

`new AWS.SNS(options = {})`  <br>

*Property Summary* <br>

`endpoint ⇒ AWS.Endpoint` <br>
An Endpoint object representing the endpoint URL for service requests.


SNS basics:
- Step 1: Create a topic
- Step 2: Create a subscription to the topic.
- Step 3: Publish a message to the topic.
- Step 4: Delete the subscription and topic.


### SQS
Amazon Simple Queue Service (Amazon SQS) is a reliable, highly-scalable hosted queue for storing messages as they travel between applications or microservices. Amazon SQS moves data between distributed application components and helps you decouple these components.

For information on the permissions you need to use this API, see Identity and access management in the Amazon Simple Queue Service Developer Guide.

You can use AWS SDKs to access Amazon SQS using your favorite programming language. The SDKs perform tasks such as the following automatically:

- Cryptographically sign your service requests.

- Retry requests.

- Handle error responses.



![img](./img/snsansSQS.png) <br>


### Key Differences: <br>

- Entity Type
  - SQS : Queue (similar to JMS, MSMQ).
  - SNS : Topic-Subscriber (Pub/Sub system).
- Message consumption
  - SQS : Pull Mechanism — Consumers poll messages from SQS.
  - SNS : Push Mechanism — SNS pushes messages to consumers.
- Persistence
  - SQS : Messages are persisted for some duration is no consumer available. The retention period value is from 1 minute to 14 days. The default is 4 days.
  - SNS : No persistence. Whichever consumer is present at the time of message arrival, get the message and the message is deleted. If no consumers available then the message is lost.
In SQS the message delivery is guaranteed but in SNS it is not.
- Consumer Type
  - SQS : All the consumers are supposed to be identical and hence process the messages in exact same way.
  - SNS : All the consumers are (supposed to be) processing the messages in different ways.
- Use Cases
  - Choose SNS if:
 1. You would like to be able to publish and consume batches of messages.
 1. You would like to allow same message to be processed in multiple ways.
 1. Multiple subscribers are needed.
   - Choose SQS if:
 1. You need a simple queue with no particular additional requirements.
 1. Decoupling two applications and allowing parallel asynchronous processing.
 1. Only one subscriber is needed.

