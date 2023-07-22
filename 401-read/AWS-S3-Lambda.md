# AWS: S3 and Lambda
## AWS S3:
### Amazon S3 (Simple Storage Service) is a scalable cloud-based storage solution provided by Amazon Web Services (AWS). It allows users to store and retrieve data over the internet with high durability, availability, and security.
### S3 is commonly used for data backup, content distribution, and as a data store for web applications.
## Name some use cases for Amazon S3:
### Data Backup and Archiving: S3 provides a reliable and durable storage solution for backing up critical data and archiving historical records. It ensures data integrity and allows easy retrieval when needed.

### Static Website Hosting: S3 can be used to host static websites, serving HTML, CSS, and media files directly to visitors. It simplifies web hosting, offers high availability, and reduces operational costs.

## Name some benefits of using Amazon S3:
### Scalability: Amazon S3 provides virtually unlimited storage capacity, allowing users to scale their storage resources up or down as needed without worrying about infrastructure management.

### Durability and Reliability: S3 automatically replicates data across multiple data centers within an AWS Region, ensuring high durability and data availability, even in the event of hardware failures.

## AWS Lambda Basics:
### what is AWS Lambda Basics:
#### AWS Lambda is a serverless compute service by Amazon Web Services (AWS) that lets you run code without managing servers. 
#### It automatically scales, executes code in response to events, and bills based on usage, making it ideal for event-driven applications and microservices.

## Name some use cases for AWS Lambdas:
#### Microservices: AWS Lambda allows developers to create small, individual functions that perform specific tasks, facilitating the development and management of microservices architectures.

#### Event-Driven Processing: Lambda functions can be triggered by various events, such as changes in data stored in Amazon S3, updates to a database, or messages from Amazon SQS, enabling event-driven processing for real-time applications.

## Describe “serverless” to a non-technical friend.:
### "Serverless" means you can run your applications without worrying about managing servers. It's like renting a ready-to-use workspace where you only pay for the time you spend there, and someone else takes care of all the maintenance, so you can focus on your work without the hassle of managing the space.

## CDN:
### What is a CDN?
#### A CDN (Content Delivery Network) is a network of servers distributed globally that caches and delivers web content, like images, videos, and files, to users from the closest server to their location. This reduces load times, improves website performance, and ensures a better user experience by reducing latency and handling traffic spikes efficiently.
### How does a CDN work with relation to the website visitor?
#### When a website visitor requests content, the CDN routes the request to the nearest server in its network, reducing the distance data travels and minimizing latency. The CDN caches the content on this server, and subsequent visitors in the same area receive the content directly from the nearby server, resulting in faster load times and a smoother browsing experience. The CDN also offloads traffic from the origin server, distributing the load and improving the website's overall performance and reliability.
### What are the benefits of employing a CDN?
- Faster Load Times: CDN caches content closer to users, reducing latency and speeding up website loading, leading to improved user experience.
- Scalability and Reliability: CDNs distribute traffic across multiple servers, handling sudden traffic spikes efficiently and increasing website's reliability and availability.
- Cost Savings: Offloading content delivery to a CDN can reduce bandwidth costs and server load, optimizing resource usage and potentially lowering infrastructure expenses.
