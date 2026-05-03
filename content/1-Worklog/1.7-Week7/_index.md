---
title: "Weekly Worklog 7"
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

| No. | Task | Start Date | End Date | Resource |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Research: Data Routing architecture and advantages of SQS FIFO in ensuring data ordering. <br> - **Project:** <br> &nbsp;&nbsp;+ Transition data flow to use SQS FIFO as a central processing buffer. | 04/20/2026 | 04/20/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 2 | - Research: Alert Debounce logic and controlling alert states based on timestamps. <br> - **Project:** <br> &nbsp;&nbsp;+ Build an algorithm to suppress repeated SNS alerts based on time-status queries from DynamoDB. | 04/21/2026 | 04/21/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 3 | - Research: Hive Partitioning mechanisms and advanced DDL commands in Amazon Athena. <br> - **Project:** <br> &nbsp;&nbsp;+ S3 Storage Upgrade: Deploy Hive Partitioning (year/month/day/appid). <br> &nbsp;&nbsp;+ Synchronize data partitions using Athena. | 04/22/2026 | 04/22/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 4 | - Research: Lambda integration with HTTP API Gateway and authentication for Client Dashboard. <br> - **Project:** <br> &nbsp;&nbsp;+ Review integration flow between API Gateway and Lambda for data retrieval. | 04/23/2026 | 04/23/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 5 | - Research: DynamoDB Time to Live (TTL) and S3 Lifecycle Management. <br> - **Project:** <br> &nbsp;&nbsp;+ Configure S3 Lifecycle Rules; create DynamoDB tables with TTL mechanism. <br> &nbsp;&nbsp;+ Package Python source code and set up SQS as an Event Trigger for Lambda. | 04/24/2026 | 04/24/2026 | [AWS Documentation](https://docs.aws.amazon.com) |

### Key Achievements in Week 7:

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

### Knowledge Gained:

* **Technical Expertise:** Gained a deep understanding of the differences between synchronous and asynchronous architectures in log processing. Mastered Hive data partitioning techniques for handling Big Data on the Cloud platform.
* **Soft Skills:** Developed advanced Python source code analysis capabilities. Honed an architectural optimization mindset to meet real-world performance and cost requirements.
