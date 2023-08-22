# Class 16 Reading Notes

## AWS EC2

1. What is an EC2 Instance?

- A virtual server used to request and provide a computer server with AWS cloud

2. Name 2 use cases for EC2.

- Run cloud-native and enterprise apps
- develop for Apple platforms

3. Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.

- With ECS you have more control over the infrastructure and deployment of your app.

## EC2 for humans

1. Where can we find EC2 on the AWS Console?

- Navigate to the services dropdown menu and click conmput to expand, click EC2

2. Explain the general difference between T2 Micro and XL.

- Both are instance types however the T2 Micro are intended for light weight workloads while T2 XL are designed to handle larger workloads and more demanding apps.

3. Explain a “Compute Cycle” to a non-technical friend.

- the compute cycle is the time it takes for a computer to do a task. Everytime you press a key on the computer keyboard the device goes through a compute cycle to process what key you just pressed and show it on the screen.

## Elastic Beanstalk

1. What is Elastic Beanstalk?

- Elastic Beanstalk is a platform for devs to use to deploy, maage and scale web apps

2. Describe the relationship between EC2 and Elastic Beanstalk.

- Elastic Beanstalk leverages EC2 to host and run apps. When you deploy an app using EBS it provisions EC2 instances for the app to run.

3. Name some benefits of using Elastic Beanstalk.

- ease of deployment, automated scaling, manages the environment including system updates and patching.
