# AWS: Cloud Servers

## AWS EC2

### What is an EC2 Instance?

An EC2 (Elastic Compute Cloud) instance is a virtual server in the Amazon Web Services (AWS) cloud. It provides resizable compute capacity in the cloud and allows you to run applications and services.

### Name 2 use cases for EC2.

- Web hosting: You can use EC2 instances to host websites and web applications, allowing you to easily scale resources based on demand.
- Data processing: EC2 instances are commonly used for data processing tasks such as data analysis, machine learning, and big data processing.

### Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.

One reason to use Amazon ECS (Elastic Container Service) instead of services like Heroku, Digital Ocean, or Render.com is that ECS provides more control and flexibility over your containerized applications. With ECS, you have granular control over the underlying infrastructure, scalability, and networking of your containers, allowing you to optimize your application's performance and cost.

## EC2 For Humans

### Where can we find EC2 on the AWS Console?

You can find EC2 in the AWS Management Console by following these steps:

- Sign in to the AWS Management Console.
- Open the "Services" menu and select "EC2" under the "Compute" section. Alternatively, you can type "EC2" in the search bar and select the EC2 service from the results.

### Explain the general difference between T2 Micro and XL.

T2 Micro and XL refer to different instance types available in EC2, and their main difference lies in the allocated resources. Here's a general comparison:

- T2 Micro: It is a small instance type with limited resources, suitable for low-traffic or lightweight applications. It provides a low baseline performance and accumulates CPU credits during idle periods, which can be used for burstable performance when needed.

- XL: "XL" is not a specific EC2 instance type, but typically represents larger instance types, such as the m5.xlarge or c5.xlarge. These instances have higher computational capacity, more CPU cores, and increased memory compared to a T2 Micro. They are better suited for applications with higher performance requirements or resource-intensive workloads.

### Explain a “Compute Cycle” to a non-technical friend.

Imagine a compute cycle as a single unit of work performed by a computer processor. It's like a small task that the computer needs to complete. The more compute cycles a computer can perform per second, the faster it can process data and execute instructions.

To put it simply, think of a compute cycle as a single step in a larger process. Just like a person walking, each step (compute cycle) moves them forward towards their destination. Similarly, a computer performs compute cycles to complete tasks, process information, and make things happen.

## Elastic Beanstalk

### What is Elastic Beanstalk?

Elastic Beanstalk is a fully managed service by AWS that makes it easier to deploy, run, and scale web applications and services. It abstracts away the underlying infrastructure complexities and automates the deployment process, allowing developers to focus more on writing code rather than managing servers.

### Describe the relationship between EC2 and Elastic Beanstalk.

Elastic Beanstalk leverages EC2 instances as the underlying infrastructure for hosting your web applications. When you deploy your application using Elastic Beanstalk, it automatically provisions and manages the necessary EC2 instances, load balancers, and networking configurations. Elastic Beanstalk takes care of the deployment, scaling, and monitoring aspects, while EC2 provides the compute resources to run the application.

### Name some benefits of using Elastic Beanstalk.

- Easy deployment: Elastic Beanstalk simplifies the process of deploying applications by handling the infrastructure setup, including load balancing, auto-scaling, and capacity provisioning.
- Automatic scaling: It can automatically scale your application based on traffic or custom-defined metrics, ensuring your application can handle varying workloads.
- Monitoring and health checks: Elastic Beanstalk provides built-in monitoring capabilities, including health checks, metrics, and log management, allowing you to easily monitor the health and performance of your application.
