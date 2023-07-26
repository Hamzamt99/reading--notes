#  AWS: Events:
## AWS SQS vs SNS:
### What is the difference betweeen SQS and SNS?
Amazon SQS (Simple Queue Service) is a message queuing service that enables decoupling of components by storing and managing messages in queues. It follows the point-to-point communication model.
Amazon SNS (Simple Notification Service) is a pub/sub (publish/subscribe) service that sends messages to multiple subscribers (endpoints) simultaneously, allowing broadcast-type communication.
In summary, SQS is for point-to-point messaging, while SNS is for pub/sub messaging.

### What are some use cases for both SNS and SQS?
#### Use cases for Amazon SQS:
- Task Queuing: Distributing tasks to worker instances for asynchronous processing, such as image or video processing.
- Decoupling Microservices: Decoupling components of a distributed system, allowing independent scaling and fault tolerance.
## AWS SNS and SQS:
### Describe how to use SQS and SNS in a “fanout” pattern:
- Create an SNS topic and subscribe multiple SQS queues to it.
- When a message is sent to the SNS topic, it will be automatically delivered to all subscribed SQS queues, enabling parallel processing of the message by multiple consumers.
- Each SQS queue can have its own set of workers to process the message independently, providing a scalable and distributed architecture for processing events.
### Explain how “push notifications” work, using SNS:
- Mobile devices register with SNS endpoints (e.g., iOS or Android devices).
- When an event occurs, a message is sent to the SNS topic, which automatically delivers it to all registered endpoints.
- SNS handles message formatting and delivery, allowing applications to send personalized and timely push notifications to mobile devices.
## SQS and SNS Basics:
### How might a large scale, distributed application make use of a Queue system like SQS?
- Decoupling Components: SQS helps decouple different components of the application, allowing them to work independently and asynchronously. This promotes loose coupling and enhances fault tolerance, as failures in one component won't directly impact others.
- Load Leveling: SQS acts as a buffer between application components, enabling efficient load leveling. When one component produces messages faster than another can consume them, SQS stores the excess messages, preventing backlogs and overloading of downstream services.
- Scaling and Elasticity: SQS can automatically scale based on the incoming message traffic. As the application load increases, SQS can handle a larger number of messages and accommodate more instances of worker processes for processing those messages.
- Batch Processing: SQS supports batch processing, allowing multiple messages to be processed together, reducing the overhead of handling individual messages and improving efficiency.



