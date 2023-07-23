# AWS: Events

**AWS SQS vs. SNS:**

**Difference:**

- SQS: Message queuing service for decoupling and asynchronous processing.
- SNS: Pub/sub messaging service for push-based message distribution.

**Use cases:**

- SQS: Decoupling, load leveling, task offloading.
- SNS: Fanout patterns, push notifications, email/SMS alerts.

**Using SQS and SNS in a "fanout" pattern:**

- SNS broadcasts messages to multiple SQS queues.

**How "push notifications" work using SNS:**

- SNS pushes messages to subscribed endpoints in real-time.

**Large scale distributed application and SQS usage:**

- SQS manages communication between components for scalability and fault tolerance.
