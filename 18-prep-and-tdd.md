## Amazon API Gateway
What is Amazon API Gateway?
Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

How does API Gateway work?
API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.
fully managed authentication and authorization layers, as well as detailed metrics and tracing for API requests.

### Benefits of Amazon API Gateway
- Map HTTP requests to specific functions in a Serverless application via an API Gateway event.
- Map WebSocket events to Serverless functions. If you are building a WebSocket API, API Gateway also lets you map its events to a Serverless function.
- Use multiple microservices to serve the same top-level API. 
- Save time with integrations: authentication, developer portal, CloudTrail, CloudWatch. API Gateway allows you to implement a fully managed authentication and authorization layer by using Amazon Cognito and Lambda custom authorizers without running your own auth systems.


### Amazon API Gateway limits
- Regional APIs: you can only have 600 regional APIs per AWS account. That’s a lot; most teams won’t reach this limit.
- ntegration timeouts: the shortest possible timeout for an integration in API Gateway is 50 ms, and the longest is 29 seconds.
- Payload size: the maximum payload size that can be returned by an API endpoint is Payload size: the maximum payload size that can be returned by an API endpoint is

## Benefits

- Efficient API development
- Performance at any scale
- Cost savings at scale
- Easy monitoring
- Flexible security controls
- RESTful API options


## DynamoDB
What is DynamoDB?
DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:

- reliable performance even as it scales;
- a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
- a small, simple API allowing for simple key-value access as well as more advanced query patterns.

DynamoDB is a particularly good fit for the following use cases:
- Applications with large amounts of data and strict latency requirements
- Serverless applications using AWS Lambda.
- Data sets with simple, known access patterns.

### Amazon DynamoDB
How it works
Amazon DynamoDB is a fully managed, serverless, key-value NoSQL database designed to run high-performance applications at any scale. DynamoDB offers built-in security, continuous backups, automated multi-Region replication, in-memory caching, and data export tools.

Use cases:
- Develop software applications
- Create media metadata stores
- Deliver seamless retail experiences
- Scale gaming platforms


Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.

Key Features:
- Type safety
- High level API
- Easy to use syntax
- Ability to transform data before saving or retrieving documents
- Strict data modeling (validation, required attributes, and more)
- Support for DynamoDB Transactions
- Powerful Conditional/Filtering Support
- Callback & Promise support
