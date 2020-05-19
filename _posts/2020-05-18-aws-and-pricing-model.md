`---
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

> On-Demand
>
>> What does on demand means ?
>> - The cost for running the instance is computed at fixed rate by the hour (or by second).
>> 
>> Why do I need it ?
>> - No commitments 
>> - No upfront payments
>> - Can increase or decrease compute capacity depending on the demands of your application
>> - Pay for only the hours you use
>>
>> When do I need it ?
>> - For low cost and flexibility without any up-front payment or long term commitment
>> - Applications with short-term, spiky, or unpredictable workloads that cannot be interrupted
>> - Applications being developed or tested for the first time
>>
>> [See On-Demand Pricing](https://aws.amazon.com/ec2/pricing/on-demand/ "EC2 On-Demand Pricing")

> Reserved

- Provides you with a capacity reservation, and offer a significant discount on the hourly charge for an instance. Contract terms are 1 to 3 years.

> Spot
   
1. Enables you to bid whatever price you want for instance capacity, providing for even greater savings if your applications have flexible start and end times.
   
2. If terminated by amazon, you will not be charged for a partial hour of usage. However, if you terminate the instance yourself, you will be charged for any hour in which the instance ran.

> Dedicated Hosts

- Physical EC2 server dedicated for your use. Dedicated hosts can help you reduce costs by allowing you to use your existing server-bound software licenses.`