## Readings: AWS: API, Dynamo and Lambda

### 1. What are serverless functions?

Serverless functions are discrete fucntions that perform as specific task. The developer is responsible for the logic while a cloud provider performs the container management. These functions are event-driven, meaning the code is only invoked when triggered by a request. AWS calls there serverless function solution Lambda.

https://www.infoworld.com/article/3406501/what-is-serverless-serverless-computing-explained.html

### 2. If you were to create a system that emulated Lambda functions, how would you do it?

I would provision containers from a cloud provider. Each container would be configured as an API endpoint that executed a function when triggered by a request. It would then respond with the results of that function.

### 3. Describe how a CDN works

A content delivery network (CDN) refers to a geographically distributed group of servers which work together to provide fast delivery of Internet content. By distributing content across servers in different locales, visitors near those servers experience faster response times.

https://www.cloudflare.com/learning/cdn/what-is-a-cdn/

### Document the following Vocabulary Terms

#### Serverless Functions

A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

https://blog.hubspot.com/website/serverless-functions

#### Cloud Storage

Cloud storage is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service.

https://aws.amazon.com/what-is-cloud-storage/

#### CDN

A content delivery network (CDN) is a group of geographically distributed servers that speed up the delivery of web content by bringing it closer to where users are.

https://www.akamai.com/our-thinking/cdn/what-is-a-cdn
