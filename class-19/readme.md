# AWS - API, Dynamo, and Lambda

Welcome to the readings section for today's topic on AWS - API, Dynamo, and Lambda. Below you will find a selection of curated reading materials, code samples, and additional resources to support your understanding of these key concepts.

**Submission Instructions:** Please review the provided guidelines for completing and submitting the assignment.

## AWS API Gateway Overview

- **What is Amazon API Gateway?**

  Amazon API Gateway is an essential fully managed service that empowers developers to create, publish, maintain, monitor, and secure APIs, irrespective of the scale.

- **Why is Amazon API Gateway an important part of the Serverless ecosystem?**

  Amazon API Gateway plays a pivotal role in the Serverless ecosystem as it enables seamless communication between serverless functions and external systems through APIs.

- **How does API Gateway integrate with other AWS services?**

  API Gateway seamlessly integrates with various AWS services like AWS Lambda, AWS DynamoDB, and more, empowering developers to build robust and scalable applications.

## AWS API Gateway

- **What are some benefits of using Amazon API Gateway?**

  - Easy API creation
  - Scalability
  - Enhanced security through authentication and authorization mechanisms
  - Efficient caching
  - Effective throttling for better control over traffic

- **What two API types might you choose from?**

  Amazon API Gateway supports two API types:

  - RESTful APIs: Ideal for traditional HTTP requests and standard CRUD operations.
  - WebSocket APIs: Perfect for real-time communication and bidirectional data flow.

## AWS DynamoDB Guide

- **What is DynamoDB?**

  DynamoDB, an AWS fully managed NoSQL database service, offers high scalability, low latency, and seamless performance, making it an excellent choice for web and mobile applications.

- **Under what circumstances would you recommend DynamoDB over MongoDB?**

  DynamoDB is recommended over MongoDB in scenarios where you need seamless scaling with virtually unlimited storage capacity and extremely low latency. It is particularly suitable for applications with unpredictable workloads or those requiring high availability.

## AWS DynamoDB

- **Explain to a non-technical friend how DynamoDB works.**

  Imagine DynamoDB as a powerful database that stores information in a manner similar to a large table, where data is organized based on unique keys. It can handle vast amounts of data rapidly and efficiently, making it the go-to option for applications needing quick access and storage of information.

## Dynamoose

- **What is Dynamoose?**

  Dynamoose is a widely used library in Node.js applications that simplifies interactions with DynamoDB. It follows an object data modeling (ODM) approach, making working with DynamoDB more intuitive and developer-friendly.

- **What are some key features of Dynamoose?**

  - Definition of models and schemas, resembling traditional databases
  - Easy querying for data retrieval
  - Built-in validation for ensuring data consistency
  - Support for hooks to execute actions before or after specific events.
