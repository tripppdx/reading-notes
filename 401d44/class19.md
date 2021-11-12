## Readings: AWS: Events

### 1. Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server

AWS API Gateway is a managed service that acts as a portal provideing access to fucntions running on AWS Lambda. Gateway provides the endpoints and acts as a trigger for the Lambda functions, which can be configured to provide CRUD functionality. ExpressJS Server is middleware that provides a web application framework for Node.js.

https://www.digitalocean.com/community/tutorials/nodejs-express-basics

### 2. List the AWS Database offerings and talk about the pros and cons of each

| Product                                           | Description                                                                                                                                  |
| ------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Amazon RDS Managed Relational Database Service    | Amazon RDS is a managed relational database service for MySQL, PostgreSQL, MariaDB, Oracle BYOL, or SQL Server.                              |
| Amazon DynamoDB NoSQL Database Service            | A serverless database for applications that need high performance at any scale.                                                              |
| Amazon Redshift Data Warehouse                    | Fast, simple, cost-effective data warehousing.                                                                                               |
| AWS Database Migration Service Database Migration | Migrate databases with minimal downtime.                                                                                                     |
| Amazon ElastiCache In-Memory Data Store           | Managed, in-memory data store services that make it easy to deploy, operate, and scale popular open source compatible in-memory data stores. |

https://aws.amazon.com/free/database/

### 3. What’s the difference between a FIFO and a standard queue?

AWS standard SQS queues guarantee at least once delivery but does not guarantee messages are delivered in the order in which they are sent. SQS Fifo queues gurantee messages ar edelivered in the corect order and that each message will only be delivered once.

https://medium.com/awesome-cloud/aws-difference-between-sqs-standard-and-fifo-first-in-first-out-queues-28d1ea5e153

### 4. How can the server be assured a message was properly received?

The server can be assured a message was properly received if the recipient replies with an acknowledgement.

### Document the following Vocabulary Terms

#### Serverless API

A serverless API is an API that uses serverless funtions to perform CRUD. Serverless functions are discrete fucntions that perform as specific task. The developer is responsible for the logic while a cloud provider performs the container management. These functions are event-driven, meaning the code is only invoked when triggered by a request. AWS calls there serverless function solution Lambda.

https://www.infoworld.com/article/3406501/what-is-serverless-serverless-computing-explained.html

#### Triggers

In AWS Lamda, a trigger is a an event that you configure to invoke your function in response to lifecycle events, external requests, or on a schedule. Each trigger acts as a client invoking your function independently

https://docs.aws.amazon.com/lambda/latest/dg/lambda-invocation.html

#### Dynamo vs Mongo

Dynamo and Mongo are both NoSQL databases.

#### Dynamoose vs Mongoose

Dynamoose and Mongoose are Object Data Modeling (ODM) librares for DyanmoDB and MongoDB respectively.
