---
title: "Week 2 Worklog"
date: 2025-09-15
weight: 2
chapter: false
pre: "<b>1.2. </b>"
---


### Week 2 Objectives

- Master **Amazon EC2** lifecycle: From AMI selection to SSH connectivity.
- Implement **Defense in Depth**: Differentiating Security Groups vs. Network ACLs (NACL).
- Gain industry insights on AI/Data trends via Cloud Day.

### Tasks to be carried out this week

| Day | Task | Start Date | Completion Date | Reference Material |
|-----|------|------------|-----------------|---------------------|
| 2 | - **Theory:** Analyzed EC2 Instance families (General Purpose vs. Compute Optimized) and processor architectures (Intel vs. AWS Graviton).<br>- **Cryptography:** Deep dive into asymmetric encryption (Key Pairs) for secure SSH access. | 09/15/2025 | 09/16/2025 | [REFER HERE](https://cloudjourney.awsstudygroup.com/) |
| 3 | - **Provisioning:** Launched EC2 Instances (Ubuntu/Amazon Linux 2) within Public Subnets.<br>- **Security Layering:**<br>&emsp;+ Configured **Security Groups** (Stateful Firewall) at the Instance level.<br>&emsp;+ Configured **NACLs** (Stateless Firewall) at the Subnet level for traffic filtering. | 09/16/2025 | 09/17/2025 | [REFER HERE](https://docs.aws.amazon.com/ec2/) |
| 4 | - **Troubleshooting:** Debugged "Connection Time Out" errors (root caused by missing Route Table entries or SG rules).<br>- Handled account verification requests to increase Service Quotas. | 09/17/2025 | 09/20/2025 | [REFER HERE](https://aws.amazon.com/support/) |
| 5 | - **Event:** Attended **AWS Cloud Day**.<br>- **Insight:** Explored Generative AI (Amazon Bedrock) use cases and Enterprise Data Analytics strategies. | 09/18/2025 | 09/18/2025 | |

### Week 2 Achievements

* Gained foundational knowledge of VPC and EC2, including their core concepts and configurations.
* Understood the necessary steps and resources required to launch an EC2 instance.
* Successfully provisioned the first compute resources and established secure remote access.
* Conceptualized the **Security Layering** model: NACL as the "Neighborhood Gate" (Subnet) vs. Security Group as the "Building Guard" (Instance).
* Broadened perspective on modern Cloud trends (GenAI/Data) to inform future architectural decisions.