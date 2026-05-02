---
title: "Weekly Worklog 6"
date: 2026-04-13
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Goals:

* Focus on researching and practicing advanced security and identity management solutions on AWS.
* Continue developing and optimizing data processing modules for the "Log Management System" project.
* Perform internal integration testing to ensure the stability of core data flows.

### Tasks Implemented This Week:

| No. | Task | Start Date | End Date | Resource |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Research: Single Sign-On (SSO) mechanisms and multi-account governance with AWS Organizations. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Setup AWS IAM Identity Center (SSO) for centralized access management. | 04/13/2026 | 04/13/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 2 | - Research: Privilege escalation risks and IAM Policy Condition Keys (e.g., SourceIp, CurrentTime). <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Configure IAM Permission Boundaries to limit maximum user privileges. <br> &nbsp;&nbsp;+ Establish IAM Roles with strict IP and time-based conditions. | 04/14/2026 | 04/14/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 3 | - Research: CIS security benchmarks and resource configuration history tracking. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Enable AWS Config; setup AWS Security Hub to track security compliance scores. | 04/15/2026 | 04/15/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 4 | - Research: Common web attacks (SQL Injection, XSS) and behavioral anomaly detection. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Configure GuardDuty for threat monitoring; deploy AWS WAF to protect applications. | 04/16/2026 | 04/16/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 5 | - Research: KMS symmetric key management and CloudTrail traceability log structures. <br> - **Project:** <br> &nbsp;&nbsp;+ Use KMS for data encryption; query CloudTrail logs using SQL via Athena. <br> &nbsp;&nbsp;+ Optimize Lambda JSON parsing code and perform integration testing for S3 data flow. | 04/17/2026 | 04/17/2026 | [AWS Documentation](https://docs.aws.amazon.com) |

### Key Achievements in Week 6:

#### 1. Infrastructure Security & Identity Management
* Gained a comprehensive understanding of AWS security by coordinating IAM Identity Center, AWS Config, CloudTrail, and AWS WAF.
* Mastered the technique of setting up "guardrails" using Permission Boundaries, preventing privilege escalation risks within the system.

#### 2. Monitoring & Threat Detection
* Successfully implemented an intrusion detection system with Amazon GuardDuty based on VPC Flow Logs and DNS Logs analysis.
* Learned how to use Security Hub to monitor account compliance levels against international standards.

#### 3. Encryption & Traceability Analysis
* Mastered the data encryption process using symmetric keys in KMS and learned to trace every system operation through CloudTrail.
* Proficiently used Amazon Athena to perform complex SQL queries directly on raw logs for auditing and reporting purposes.

#### 4. Project Progress: "Log Management System"
* Successfully optimized Lambda function performance, enabling faster and more accurate processing of JSON-formatted logs.
* Ensured that the data flow—from collection by CloudWatch Agent to Lambda filtering (Error/Warning) and storage in S3—operates stably through integration tests.

### Knowledge Gained:

* **Technical Expertise:** Mastered the coordination of AWS security services to create a multi-layered defense system. Proficient in using command-line environments (WSL) to configure complex IAM policies that the Console interface cannot handle quickly.
* **Soft Skills:** Developed a "Security by Design" mindset. Improved troubleshooting skills for permission errors and source code optimization in real-world environments.