---
layout: post
title: "EC2 & Pricing Model"
date: 2020-05-18  09:00:00 +0800
categories: AWS
---

### Amazon Elastic Compute Cloud
> What is Elastic Compute Cloud ?

- A web service that provies resizable compute capacity in the cloud

> Why do I need it ?

- Because it reduces the time required to obtain and boot new server instances to minutes, allowing you  to quickly scale capacity, both up and down

> When do I need it ?
- As your computing requirements change.

### EC2 Pricing Model

#### On-Demand
  
> What does on-demand offers ?
- The cost for running the instance is computed at fixed rate by the hour (or by second).
 
> Why do I need it ?
- No commitments 
- No upfront payments
- Can increase or decrease compute capacity depending on the demands of your application
- Pay for only the hours you use

> When do I need it ?
- For low cost and flexibility without any up-front payment or long term commitment
- Applications with short-term, spiky, or unpredictable workloads that cannot be interrupted
- Applications being developed or tested for the first time

[See On-Demand Pricing](https://aws.amazon.com/ec2/pricing/on-demand/ "EC2 On-Demand Pricing")

#### Reserved

> What does reserved offers ?
- Significant discount on the hourly charge compared to On-Demand
- When assigned to specfic AZ, they provide a capacity reservation i.e. always be able to launch instances whenever needed

> Why do I need it ?
- It provide significant savings

> When do I need it ?
- Application with steady state usage
- Applications that may require reserve capactiy
- Customer able to commit to using EC2 over 1 - 3 year term to reduce their total computing cost

#### Spot

> What does Spot offers ?
- Enables you to bid whatever price you want for instance capacity
- Up to a 90% discount compared to On-Demand prices
- If terminated by amazon, you will not be charged for a partial hour of usage. However, if you terminate the instance yourself, you will be charged for any hour in which the instance ran.

> Why do I need it ?
- Providing for even greater savings if your applications

> When do I need it ?
- Application can have flexible start and end times.
- Urgent computing needs for large amount of addtional capacity
- For stateless, fault tolerant, or flexibile application. For example: big data, containerized workloads, CI/CD, web servers, high-performance computing and other test & development work loads

#### Dedicated Hosts

> What does Dedicated Host offers ?
- Physical EC2 server
- Can be purchase On-Demand (hourly)
- Can be purchase as a Reservation for up to 70% off the On-Demand price

> Why do I need it?
- Help you reduce costs by allowing you to use your existing server-bound software licenses.

> When do I need it ?
- Server-bound software licenses