---
title: "Worklog Week 7"
date: 2026-04-20
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:

* Refactor the entire project to an advanced Serverless architecture to resolve bottleneck issues.
* Implement a Message Queue mechanism to coordinate stable log data flows.
* Optimize storage structure and Big Data queries on S3 using Hive Partitioning and Amazon Athena.

### Tasks implemented this week:

| Task | Start Date | Completion Date | Reference |
| :--- | :--- | :--- | :--- |
| - Data Routing Refactoring: Analyzing and transitioning the data flow to use SQS FIFO as a processing buffer. | 20/04/2026 | 20/04/2026 | https://cloudjourney.awsstudygroup.com |
| - Alert Debounce Logic Research: Building an algorithm to suppress repeated SNS alerts based on time-status queries from DynamoDB. | 21/04/2026 | 21/04/2026 | https://cloudjourney.awsstudygroup.com |
| - S3 Storage Upgrade: Deploying Hive Partitioning (year/month/day/appid) and researching Athena DDL commands for partition synchronization. | 22/04/2026 | 22/04/2026 | https://cloudjourney.awsstudygroup.com |
| - API Endpoint Analysis: Reviewing the integration flow between HTTP API Gateway and Lambda for retrieving data for the Client Dashboard. | 23/04/2026 | 23/04/2026 | https://cloudjourney.awsstudygroup.com |
| - Core Storage Infrastructure Deployment: Configuring S3 buckets with the new partition structure, setting Lifecycle Rules, and creating DynamoDB tables with TTL. | 24/04/2026 | 24/04/2026 | https://cloudjourney.awsstudygroup.com |
| - SQS and Lambda Integration: Packaging Python source code, configuring SQS as an event trigger, and establishing IAM Roles for system integration. | 24/04/2026 | 24/04/2026 | https://cloudjourney.awsstudygroup.com |



### Week 7 Outcomes:

#### 1. Advanced System Architecture
* Successfully transitioned from a traditional log collection model to a distributed Serverless architecture, utilizing SQS FIFO queues to guarantee message ordering and system load capacity.
* Mastered JSON parsing within the Lambda Consumer to simultaneously distribute data into cold storage (S3) and hot storage (DynamoDB).

#### 2. Alert Management Optimization
* Completely resolved the email "bombing" issue using an Alert Debounce algorithm, allowing for the control of SNS alert frequency within a 15-minute window.

#### 3. Large-Scale Data Management
* Established a Hive Partitioning structure on S3, which optimized storage space and significantly increased query speeds for Amazon Athena.
* Successfully implemented a Time to Live (TTL) mechanism on DynamoDB to automatically clean up status logs, maintaining table performance and reducing costs.

#### 4. Infrastructure Deployment & Integration
* Successfully deployed and connected event flows between core services (SQS, Lambda, S3, DynamoDB, SNS) through the configuration of strict and secure IAM Role policies.



### Accumulated Knowledge:

* **Technical Skills:** Gained a deep understanding of the differences between synchronous and asynchronous architectures in log processing. Mastered Hive data partitioning techniques for handling Big Data on the Cloud platform.
* **Soft Skills:** Developed advanced Python source code analysis capabilities. Honed an architectural optimization mindset to meet real-world performance and cost requirements.