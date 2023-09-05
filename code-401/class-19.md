# Class 19 Reading Notes

## AWS SQS ns SNS

1. What is the difference betweeen SQS and SNS?

- SNS is a public-subscribe service while SQS is a queuing service. Amazon SNS (simple notification service) lets you send messages (individual or bulk) to a large number of recipients. It is a way to send push notifications to subscribers. SQS (simple queue service) is where messages are sent to a queue and one or more consumers can poll the queues and process the messages.

2. What are some use cases for both SNS and SQS?

- SNS can be used for event notifications, app alerts, email and sms notifications, fan-out architectures, decoupling publishers and subscribers (allows systems to evolve independently)

- SQS can be used for workload decoupling, load leveling, batch processing, error handling, task queues and buffering

## AWS SNS vs SQS

1. Describe how to use SQS and SNS in a “fanout” pattern.

- fan out pattern allows you to broadcast a message or notification to subscribers with scalability. Create an SNS topic, add subscribers, create SQS queues, publish messages, configure SQS consumers

2. Explain how “push notifications” work, using SNS.

- SNS allows you to sned real-time messages or alerts to endpoints; set up the SNS topic, configure subsribers, register devices, publish messages

## SQS and SNS Basics

1. How might a large scale, distributed application make use of a Queue system like SQS?

- Use of SQS can help enhance scalability and reliability. Differenet components need to communicate with each other asynchronously and SQS allows flexibility for this. SQS allows to distribute workloads across multiple consumers. SQS can scale to handle increased amounts of messages and tasks in the queue. SQS allows for asynchronous tasks to be queued and processed independently from the user-facing components.