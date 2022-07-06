# Code 401 - Class 17 - AWS: S3 and Lambda

## [AWS S3](https://aws.amazon.com/s3/)

### What is Amazon S3?

- Amazon Simple Storage Service is an object storage service that provides scalability, data availability, security, and performance

### Name some use cases for Amazon S3

- Back up and restore data
- Run cloud-native apps
- Build a "data lake", and then use AWS services to run data analytics, AI, machine learning, etc. to gain insights

### Name some benefits of using Amazon S3

- Offers cost-effective storage and user-friendly management features to help customers store and analyze data

## [AWS Lambda Basics](https://www.serverless.com/aws-lambda)

### What is AWS Lambda?

- A serverless computing service that allows customers to create functions (self-contained apps) and upload them to Lambda - which then executes those functions

### Name some use cases for AWS Lambdas

- Scalable API's
- Data processing (can be integrated with database software like DynamoDB)

### Describe “serverless” to a non-technical friend

- "Serverless" does not mean there are no servers involved, but rather that a customer does not need to maintain their own servers that are required to run the functions they upload. All infrastructure--including servers, OS, network layer--is taken care of by Lambda

## [CDN](https://cyberhoot.com/cybrary/content-delivery-network-cdn/)

### What is a CDN?

- Content Delivery Network - group of servers distributed geographically, to ensure fastest possible delivery of content to users.

### How does a CDN work with relation to the website visitor?

- CDN copies pages of a website to a network of servers that are spread out geographically - caching contents of the site
- User requests a webpage - CDN redirects the request to a server in the CDN that is closest to the user

### What are the benefits of employing a CDN?

- Speeds up delivery of internet content
- Helps protect websites from cyber attacks

[Video - What is a CDN?](https://youtu.be/Bsq5cKkS33I)

[Back to Home](../README.md)
