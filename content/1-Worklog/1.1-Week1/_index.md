---
title: "Weekly Worklog 1"
date: 2026-03-09
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Week 1 Goals:

* Research foundational documentation regarding core AWS service architectures.
* Directly perform hands-on lab sequences to grasp real-world system operational workflows.
* Establish a secure management environment and optimize costs from the very beginning.

### Tasks Implemented This Week:

| No. | Task | Start Date | End Date | Resource |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Research: Root account security, differences between Root User and IAM User. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Initialize account, set up Virtual MFA for Root. <br> &nbsp;&nbsp;+ Create IAM Admin Group/User. <br> &nbsp;&nbsp;+ Customize Console (Region, Dashboard Widgets). | 03/09/2026 | 03/09/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 2 | - Research: Pricing mechanisms (Free Tier, Pay-as-you-go) and AWS Support plans. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Configure 4 types of AWS Budgets (Cost, Usage, RI, Savings Plans). <br> &nbsp;&nbsp;+ Practice the Support Case creation process. | 03/10/2026 | 03/10/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 3 | - Research: Advanced permissions with IAM Roles and AWS CLI (Command Line Interface). <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Create Roles for Admin/Operator and practice Switch Role. <br> &nbsp;&nbsp;+ Initialize Cloud9 IDE and interact with the system via CLI. | 03/11/2026 | 03/11/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 4 | - Research: Amazon VPC architectural components (Subnets, IGW, NAT Gateway, Route Table). <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Design VPC: Configure Public/Private Subnets. <br> &nbsp;&nbsp;+ Establish Security Group shields. <br> &nbsp;&nbsp;+ Simulate a secure Site-to-Site VPN connection. | 03/12/2026 | 03/13/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 5 | - Research: EC2 services (Instance Types, AMI, EBS) and security Best Practices. <br> - **Project Hands-on (Log Management):** <br> &nbsp;&nbsp;+ Deploy EC2 servers (Linux & Windows). <br> &nbsp;&nbsp;+ Install LAMP stack and Node.js applications. <br> &nbsp;&nbsp;+ Attach IAM Roles to EC2 for secure S3 access without Access Keys. | 03/13/2026 | 03/13/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |

---

### Key Achievements in Week 1:

#### 1. Account Management & Security
* Completed Root account protection using MFA. Implemented a secure management model via Admin Users and Admin Groups.
* Analyzed and clearly understood the differences between AWS Support plans (Basic, Developer, Business, Enterprise) and the troubleshooting workflow via Support Cases.
* Mastered the **Switch Role** mechanism to manage cross-account access without sharing login credentials.

#### 2. Cost Control
* Successfully established an automated budget alert system for 4 core categories: Cost, Usage, Reserved Instances (RI), and Savings Plans.
* Configured alert thresholds at 80% and 100% to proactively control cloud resources.

#### 3. Network Infrastructure & Connectivity
* Successfully built an isolated network environment (VPC) with full navigation components (Route Table) and security shields (Security Group).
* Implemented a system allowing internal servers (Private Subnet) to access the internet securely via NAT Gateway and simulated secure VPN connectivity between On-premises and AWS.

#### 4. Virtual Servers & Applications (Project)
* Deployed and managed EC2 instances on both Linux and Windows platforms. Mastered tasks such as: creating Snapshots, packaging Custom AMIs, and writing Policies to restrict Instance Types/Regions.
* Applied security **Best Practices**: Used IAM Roles attached directly to EC2 instances to allow applications to access S3 automatically, completely eliminating the risk of exposing Access Keys/Secret Keys in the source code.
* Became proficient in using the **AWS Cloud9** development environment and the Command Line Interface (CLI) to query and manage resources.

---

### Knowledge Gained:

* **Technical Expertise:** Gained a deep understanding of operational mechanisms ranging from virtualized physical infrastructure (EC2, VPC) to logical security layers (IAM, Security Group). Reinforced the mindset of designing secure and cost-optimized systems on Cloud platforms through complex permission scenarios.
* **Soft Skills:** Improved the ability to read and comprehend technical documentation (AWS Documentation), enhanced troubleshooting skills during network infrastructure configuration, and developed a professional, independent reporting style.