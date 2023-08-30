# Class 18 Reading Notes

## AWS API Gateway Overview

1. What is Amazon API Gateway?

- A managed service that allows devs to define the HTTP endpoints of a REST API or a websocket API and connect those endpoints with the corresponding backend business logic. Also handles authentication, access contor, monitoring, and tracing API requests

2. Why is Amazon API Gateway an important part of the Serverless ecosystem?

- Amazon API Gateway allows for a fully functioning customer-facing app without the dev having to maintain a single layer which allows for scalability, low maintenance and low cost due to low overhead.

3. How does API Gateway integrate with other AWS services?

- The integrations with AWS Lambda, AWS SNS, and Amazon Cognito allow for a fully managed authentication and authorization layers and detailed tracing for API requests.

## AWS API Gateway

1. What are the some benefits of using Amazon API Gateway?

- Efficient API development - run multiple versions of the same API at the same time with API gateway allowing you to iterate, test and release new versions.
- Performance - use of Amazon CloudFront provides end users with the lowest latency for API reqs and res'
- Easy Monitoring - API Gateway dashboard allows you to monitor performance metrics and info on API calls, data latency and error rates
- Flexible security - AWS Identity and IAM alows you to authorize access to APIs

2. What two API types might you choose from?

- RESTful APIs and WebSocket APIs - **RESTful** is optimized for serverless workloads and HTTP backends using HTTP APIs - **WebSocket** allows you to build real-time-two-way communication apps like chat apps. API Gateway maintains connection to handle message transfers between backend and clients

## AWS DynamoDB Guide

1. What is DynamoDB?

- DynamoDB is a hosted NoSQL database that offers reliable performance as it scales, experience management and simple API allowing for simple key-value access. Handles apps with large amounts of data and strict latency requirements, is compatable with AWS Lambda for serverless app building and simple key-value access patterns.

2. Under what circumstances would you recommend DynamoDB over MongoDB?

- DynamoDB is designed for scalability and auto sharding while MongoDB requires more manual effort. DynamoDB is fully managed by AWS while MongoDB is mostly managed but still requires effort from the dev. DynamoDB is good for building a fully serverless app.

## AWS DynamoDB

1. Explain to a non-technical friend how DynamoDB works.

- DynamoDB is like a super organized spreadsheet with multiple layers that work together and are self managed so you don't have to worry about manually moving things around and organizing them everytime something new is added. Each piece of data in the spreadsheet also has a special code attached to it so the DB knows exactly where to find it when the user requests it.

## Dynamoose

1. What is Dynamoose?

- A modeling tool for DynamoDB that is similar to Mongoose.

2. What are some key features of Dynamoose?

- Type safety, high level API, easy to use syntax, ability to transform data before saving and retrieving items, strict data modeling, callback and promise support, AWS support
