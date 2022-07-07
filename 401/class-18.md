# Code 401 - Class 18

## AWS: API, Dynamo and Lambda

### [AWS API Gateway Overview](https://www.serverless.com/guides/amazon-api-gateway)

**What is Amazon API Gateway?**

- Allows developers to define HTTP endpoints of a REST or WebSocket API, and connect those endpoints with backend business logic - while handling auth, acl, etc.

**Why is Amazon API Gateway an important part of the Serverless ecosystem?**

- It allows for truly serverless architecture, by triggering execution of a serverless function in response to an HTTP request

**How does API Gateway integrate with other AWS services?**

- Direct integration can be configured in the API Gateway user interface (or through API Gateway's own API) to:
- Invoke a Lambda function
- Invoke another HTTP endpoint
- Return a mock response generated within API Gateway

### [AWS API Gateway](https://aws.amazon.com/api-gateway/)

**What are the some benefits of using Amazon API Gateway?**

- Efficient API development
- Scalability
- Flexible security
- Easy monitoring

**What two API types might you choose from?**

- RESTful API or WebSocket API

### [AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)

**What is DynamoDB?**

- A NoSQL database offered by AWS

**Under what circumstances would you recommend DynamoDB over MongoDB?**

- Need ability to scale to any size
- Need to integrate with other AWS services

### [AWS DynamoDB](https://aws.amazon.com/dynamodb/)

**Explain to a non-technical friend how DynamoDB works.**

- DynamoDB is a NoSQL database that is fully managed by AWS, to help developers focus on the functionality of their app and the data itself. It brings a lot of services with it, including built-in security, continuous backups, and data export tools.

### [Dynamoose](https://dynamoosejs.com/getting_started/Introduction/)

**What is Dynamoose?**

- Dynamoose is to DynamoDB as Mongoose is to MongoDB. It is a modeling tool for Amazon's DynamoDB database

**What are some key features of Dynamoose?**

- Type safety
- High level API
- Easy to use syntax
- Ability to transform data before saving or retrieving documents
- Strict data modeling (validation, required attributes, and more)
- Support for DynamoDB Transactions
- owerful Conditional/Filtering Support
- Callback & Promise support

[Back to Home](../README.md)
