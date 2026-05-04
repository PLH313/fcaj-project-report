---
title: "Week 3 Worklog"
date: 2026-03-23
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

* Focus on optimizing application performance through caching and content delivery solutions.
* Expand advanced network infrastructure and implement centralized system management solutions.
* Explore advanced Infrastructure as Code (IaC) features in preparation for the group project.

### Tasks implemented this week:

| No. | Tasks | Start Date | End Date | Resource |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Research: In-memory caching mechanisms, comparing Redis and Memcached. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Initialize Amazon ElastiCache (Redis Cluster). <br> &nbsp;&nbsp;+ Use AWS SDK to perform high-performance data read/write operations. | 03/23/2026 | 03/23/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 2 | - Research: Hub-and-spoke architecture with Transit Gateway and inter-region connectivity models. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Set up VPC Peering and Transit Gateway. <br> &nbsp;&nbsp;+ Configure Site-to-Site VPN connections. | 03/24/2026 | 03/24/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 3 | - Research: Route 53 Resolver for Hybrid networks and Content Delivery Network (CDN) principles. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Configure CloudFront Distributions with Cache Behaviors. <br> &nbsp;&nbsp;+ Deploy Lambda@Edge at global edge locations. | 03/25/2026 | 03/25/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 4 | - Research: Large-scale server management methods without opening ports 22/3389. <br> - **Hands-on:** <br> &nbsp;&nbsp;+ Use Systems Manager (SSM) Run Command for bulk execution. <br> &nbsp;&nbsp;+ Connect securely to instances via Session Manager. | 03/26/2026 | 03/26/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 5 | - Research: CloudFormation Custom Resources using Lambda triggers. <br> - **Project:** <br> &nbsp;&nbsp;+ Group sync to finalize RDS/DynamoDB separation for the project. <br> &nbsp;&nbsp;+ Finalize data flow diagrams for Frontend (S3/CloudFront) and Backend. | 03/27/2026 | 03/27/2026 | [AWS Documentation](https://docs.aws.amazon.com) |

### Key Achievements in Week 3:

#### 1. Performance Optimization & Distribution
* Successfully understood and implemented in-memory data storage with ElastiCache - Redis, significantly reducing the load on primary databases.
* Mastered CloudFront Distribution and Lambda@Edge configuration techniques to optimize user experience across different geographic locations.

#### 2. Hybrid Network Infrastructure & Security
* Gained proficiency in Hybrid network design by combining Transit Gateway and VPN to secure traffic between on-premises and cloud environments.
* Successfully researched DNS query forwarding mechanisms through Route 53 Resolver.

#### 3. Centralized Server Management
* Proficiently used AWS Systems Manager for patch management and bulk command execution on Windows EC2 servers.
* Completely eliminated the need for Bastion Hosts by implementing Session Manager, reducing security risks associated with opening direct management ports (22/3389).

#### 4. Infrastructure as Code & Project Shaping
* Accessed advanced CloudFormation features, specifically using Lambda as Custom Resources to initialize complex assets.
* Finalized project architecture: Using S3/CloudFront for the Frontend, Lambda/EC2 for core processing, and a hybrid RDS/DynamoDB approach for storage optimization.

### Knowledge Gained:

* **Technical Expertise:** Deeply understood system optimization methods through caching and global content delivery networks. Developed a modern server management mindset without the need for Bastion Hosts.
* **Soft Skills:** Developed a professional infrastructure automation mindset. Enhanced team coordination and system architecture planning skills for practical projects.
