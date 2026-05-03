---
title: "Weekly Worklog 4"
date: 2026-03-30
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:

* Focus on monitoring solutions and server system cost optimization.
* Practice application packaging and deployment using Container technology.
* Finalize the topic and build the core architecture for the "Log Management System" project.

### Tasks implemented this week:

| No. | Task | Start Date | End Date | Resource |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Research: Event-driven mechanisms and task scheduling with AWS Lambda. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Program Lambda to automatically start/stop EC2 instances based on usage hours to optimize costs. | 03/30/2026 | 03/30/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 2 | - Research: Docker architecture, Image lifecycle management, and Amazon ECR. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Package Web Server and Database applications using Docker. <br> &nbsp;&nbsp;+ Manage and store application images on Amazon ECR. | 03/31/2026 | 03/31/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 3 | - Research: System monitoring metrics and centralized logging mechanisms. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Configure CloudWatch Metrics, Logs, and set up Alarms. <br> &nbsp;&nbsp;+ Build visual monitoring Dashboards for resources. | 04/01/2026 | 04/01/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 4 | - Research: "Right-sizing" concepts and interpreting AWS Compute Optimizer recommendations. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Deploy CW Agent with Compute Optimizer to select ideal EC2 configurations. <br> &nbsp;&nbsp;+ Enable VPC Flow Logs to monitor IP network traffic. | 04/02/2026 | 04/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 5 | - Research: Large-scale Cloud-based log management architectures. <br> - **Project:** <br> &nbsp;&nbsp;+ Finalize project construction based on the trio: CloudWatch, Lambda, and S3. <br> &nbsp;&nbsp;+ Design the log data flow from collection to long-term storage. | 04/03/2026 | 04/03/2026 | [AWS Documentation](https://docs.aws.amazon.com) |

### Key Achievements in Week 4:

#### 1. Container Technology & Image Management
* Mastered core knowledge of application containerization using Docker.
* Proficient in managing cloud image registries via Amazon Elastic Container Registry (ECR).

#### 2. System Monitoring & Measurement
* Understood and implemented basic to advanced monitoring tools with Amazon CloudWatch.
* Developed the ability to analyze detailed network traffic entering and leaving the VPC via VPC Flow Logs to detect infrastructure anomalies.

#### 3. Resource & Cost Optimization
* Formed a Cost Optimization mindset by automating operational tasks using AWS Lambda.
* Learned how to use real-world data from CloudWatch Agent to perform "Right-sizing," assisting in selecting the most cost-effective and high-performance server configurations.

#### 4. Project Architecture Definition
* Established the core data flow for the final project: Using CloudWatch for centralized collection, Lambda for event processing, and S3 as long-term storage.

### Knowledge Gained:

* **Technical Expertise:** Recognized the importance of continuous monitoring and resource optimization based on real data (Data-driven). Mastered the process of transitioning application deployment from Local environments to the Cloud using Containers.
* **Soft Skills:** Developed problem-solving skills through automation. Enhanced teamwork abilities in discussing and finalizing system architecture decisions.
