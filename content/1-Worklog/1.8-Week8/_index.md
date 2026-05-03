---
title: "Weekly Worklog 8"
date: 2026-04-27
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:

* Finalize security architecture and user authentication for the entire project system.
* Implement identity management solutions and secure application interfaces.
* Conduct comprehensive End-to-End system testing and package the final internship report.

### Tasks implemented this week:

| No. | Task | Start Date | End Date | Resource |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Research: Authentication and Authorization models for management Dashboard systems. <br> - **Project:** <br> &nbsp;&nbsp;+ Analyze and plan user authentication methods for the Log management Dashboard. | 04/27/2026 | 04/27/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 2 | - Research: API security mechanisms and centralized identity management. <br> - **Project:** <br> &nbsp;&nbsp;+ Deploy Amazon Cognito for user identity management. | 04/28/2026 | 04/28/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 3 | - Research: Benefits of AWS App Runner for running web apps without managing servers. <br> - **Project:** <br> &nbsp;&nbsp;+ Deploy the management application on the AWS App Runner platform. | 04/29/2026 | 04/29/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 4 | - **Project:** <br> &nbsp;&nbsp;+ Conduct comprehensive End-to-End testing from EC2 to the Dashboard. <br> &nbsp;&nbsp;+ Fix Athena partition synchronization and fine-tune final IAM permissions. | 04/30/2026 | 05/01/2026 | |
| 5 | - **Project:** <br> &nbsp;&nbsp;+ Synthesize technical documentation and draw final data flowcharts. <br> &nbsp;&nbsp;+ Finalize internship report. | 05/01/2026 | 05/01/2026 | |

### Key Achievements in Week 8:

#### 1. Security & User Authentication
* Successfully implemented identity management with Amazon Cognito, allowing users to securely log into the log management Dashboard.
* Mastered setting up application interface security, ensuring log data is only accessible by authenticated users.

#### 2. Modern Application Operations
* Mastered the rapid deployment process via AWS App Runner, automating infrastructure for web apps and APIs without the need for server management.

#### 3. Completed End-to-End Data Flow
* The system passed load and logic tests: Log from EC2 -> SQS -> Lambda -> S3 & DynamoDB -> API Gateway -> Dashboard displayed smoothly.
* Completely resolved remaining Athena partition synchronization errors and final IAM permission issues.

#### 4. Internship Wrap-up
* Completed a comprehensive internship report reflecting the entire journey from learning basic services to building a complex Serverless Event-driven architecture.

### Knowledge Gained:

* **Technical Expertise:** Clearly understood how to integrate Authentication security layers into real-world Cloud systems. Gained a holistic view of the project development lifecycle from architectural design to product packaging.
* **Soft Skills:** Refined skills in information synthesis and technical report writing. Strengthened independent work capabilities and time management to meet project deadlines.
