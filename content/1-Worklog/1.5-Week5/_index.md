---
title: "Week 5 Worklog"
date: 2026-04-06
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Design, build, and secure a fully Serverless document management system on AWS.
* Optimize performance, security, and distribution speed for web applications.
* Implement core Event-driven data processing flows for the "Log Management System" project.

### Tasks implemented this week:

| No. | Task | Start Date | End Date | Resource |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Research: Serverless architecture, Partition Key/Sort Key design for DynamoDB. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Initialize DynamoDB for metadata storage. <br> &nbsp;&nbsp;+ Program AWS Lambda functions for data CRUD operations. | 04/06/2026 | 04/06/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 2 | - Research: User authentication flows and storage-at-rest security. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Configure Cognito via Amplify for User Management. <br> &nbsp;&nbsp;+ Setup S3 buckets and policies for secure file uploads. | 04/07/2026 | 04/07/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 3 | - Research: RESTful API design with Gateway and AWS SAM template structure. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Deploy API Gateway to connect Frontend and Backend. <br> &nbsp;&nbsp;+ Use AWS SAM for resource deployment automation. | 04/08/2026 | 04/08/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 4 | - Research: In-flight data encryption and Content Delivery Networks (CDN). <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Provision SSL via ACM, configure Route 53 and CloudFront. <br> &nbsp;&nbsp;+ Optimize access latency for the static website. | 04/09/2026 | 04/09/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 5 | - Research: Data synchronization via DynamoDB Streams and search indexing. <br> - **Project:** <br> &nbsp;&nbsp;+ Install CloudWatch Agent on EC2; program Lambda for log filtering. <br> &nbsp;&nbsp;+ Configure S3 Lifecycle Rules and sync OpenSearch for searchability. | 04/10/2026 | 04/10/2026 | [AWS Documentation](https://docs.aws.amazon.com) |

### Key Achievements in Week 5:

#### 1. Serverless Systems & Web Apps
* Mastered the Serverless model, understanding the coordination between Frontend, API Gateway, AWS Lambda, and DynamoDB for a complete application.
* Successfully tested API flows using Postman before integration into the official web interface.

#### 2. Infrastructure as Code (IaC) Management
* Equipped with professional infrastructure programming skills using AWS SAM, enabling bulk packaging and deployment of resources instead of manual configuration.

#### 3. Security & Distribution Optimization
* Learned to use AWS Certificate Manager (ACM) to issue SSL/TLS certificates, enhancing in-flight encryption security.
* Mastered domain routing via Route 53 and optimized page load speeds using CloudFront CDN.

#### 4. Project Core: "Log Management System"
* Completed the automated data ingestion core: Logs from EC2 are pushed by CloudWatch Agent, triggering Lambda for data normalization and secure storage in S3.
* Successfully implemented long-term cost optimization by automatically transitioning old logs to the S3 Glacier storage class.

### Knowledge Gained:

* **Technical Expertise:** Mastered Event-driven architecture and real-time data synchronization between DynamoDB and OpenSearch. Gained deep insights into modern cloud-based website security processes.
* **Soft Skills:** Developed system-level thinking by combining discrete services into a unified Serverless solution. Enhanced practical application deployment planning and testing skills.
