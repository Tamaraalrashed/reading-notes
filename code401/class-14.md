# AWS: Cloud Servers

## Review, Research, and Discussion

### What’s the difference between a FIFO and a standard queue?

Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue. FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue. <br>

### How can the server be assured a message was properly received?

The server will generate a queue once the client connect to internet he will get all massages<br>

### What classic design pattern is best represented by event driven programming?

Event Notification.<br>

### How do you test an event driven system?

Unit tests, service tests, end-to-end tests.<br>


## Terms

### FIFO Queue

FIFO (First-In-First-Out) queues are designed to enhance messaging between applications when the order of operations and events is critical, or where duplicates can't be tolerated.<br>

### Pub/Sub

Publish/subscribe messaging, or pub/sub messaging, is a form of asynchronous service-to-service communication used in serverless and microservices architectures. In a pub/sub model, any message published to a topic is immediately received by all of the subscribers to the topic.<br>

## Preparation Materials


Amazon Simple Queue Service (SQS) and Amazon SNS are both messaging services within AWS, which provide different benefits for developers. Amazon SNS allows applications to send time-critical messages to multiple subscribers through a “push” mechanism, eliminating the need to periodically check or “poll” for updates.

<br>

![img](./img/snsansSQS.png)
