---
layout: post
title: "EC2 & Pricing Model"
date: 2020-05-18  09:00:00 +0800
categories: AWS
---

## Amazon Elastic Compute Cloud
- A web service that provies resizable compute capacity in the cloud. EC2 reduces the time required to obtain and boot new server instances to minutes, allowing you  to quickly scale capacity, both up and down, as your computing requirements change.

## Pricing Model
1. On Demand
   1. Fixed rate by the hour (or by second) with no commitment.
2. Reserved
   1. Provides you with a capacity reservation, and offer a significant discount on the hourly charge for an instance. Contract terms are 1 to 3 years.
3. Spot
   1. Enables you to bid whatever price you want for instance capacity, providing for even greater savings if your applications have flexible start and end times.
   2. If terminated by amazon, you will not be charged for a partial hour of usage. However, if you terminate the instance yourself, you will be charged for any hour in which the instance ran.
4. Dedicated Hosts
   1. Physical EC2 server dedicated for your use. Dedicated hosts can help you reduce costs by allowing you to use your existing server-bound software licenses.