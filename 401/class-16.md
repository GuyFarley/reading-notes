# Code 401 - Class 16 - AWS: Cloud Servers

## [AWS EC2](https://aws.amazon.com/ec2/)

### What is an EC2 Instance?

- It is a combination of CPU, memory, storage, and networking capacity available to AWS customers of EC2 (Amazon Elastic Compute Cloud)

### Name 2 use cases for EC2

- Running cloud-native applications
- Training and deploying machine learning apps

### Provide 1 reason to use ECS instead of Heroku

- Much higher control over security and storage options, with access to many tools and customer support that Heroku may not provide

## [EC2 For Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)

### Where can we find EC2 on the AWS Console?

- First option listed under the "Compute" section on AWS Console

### Explain the general difference between T2 Micro and XL

- T2 Micro has minimal vCPU and Memory capacity, while T2 XL has quite a bit of both

### Explain a “Compute Cycle” to a non-technical friend

## [Elastic Beanstalk](https://www.youtube.com/watch?v=SrwxAScdyT0)

### What is Elastic Beanstalk?

- A service provided by AWS that deploys, manages, and scales web apps and services for the customer

### Describe the relationship between EC2 and Elastic Beanstalk

- Elastic Beanstalk uses EC2 for creating an instance, and the user can then upload their code to it. Then Elastic Beanstalk handles the rest of the deployment and management of the user's app

### Name some benefits of using Elastic Beanstalk

- This takes the responsibility of managing and maintaining an application off the developer so they can focus on building the program instead
- Automatically load balances and scales the customer's app so they can be sure it's always available
- Allows customer to maintain full control of their E.B. configurations, and therefore their app

[Back to Home](../README.md)
