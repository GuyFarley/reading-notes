# Code 401 - Class 19

## AWS: Events

### [AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

**What is the difference betweeen SQS and SNS?**

- SQS (Simple Queue System) is a distributed queueing service, while SNS (Simple Notification Service) is a distributed publish-subscribe service. A few differences:
  - SQS uses a pull mechanism (consumers poll messages from SQS) while SNS uses a push mechanism (pushes messages to consumers)
  - SQS uses data persistence (up to 14 days) while SNS does not persist data
  - With SQS, all consumers are supposed to process messages in the exact same way - while with SNS all consumers are expected to process messages differently

**What are some use cases for both SNS and SQS?**

SNS Use Cases:

- Publish and consume batches of messages
- A message needs to be processed in multiple ways
- If multiple subscribers are needed

SQS Use Cases:

- When a simple queue is needed
- Decouple to applications and allow async processing
- If only one subscriber is needed

### [AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)

**Describe how to use SQS and SNS in a “fanout” pattern.**

- SNS publishes messages to a topic that can then be delivered to many subscribers of that topic
- SQS doesn't really work with the same "fanout" pattern - messages in a queue are typically processed by a single consumer

**Explain how “push notifications” work, using SNS.**

- Notifications are simply messages that get published (or "pushed") upon a certain event, and anyone subscribed to that topic (for instance, the user of a phone app) will receive that notification

### [SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)

**How might a large scale, distributed application make use of a Queue system like SQS?**

- SQS standard queue - highly scalable
- FIFO queue - not as scalable, but processes messages exactly once, in order

[Back to Home](../README.md)
