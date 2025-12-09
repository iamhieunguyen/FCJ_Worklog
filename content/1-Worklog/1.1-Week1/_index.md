---
title: "Week 1 Worklog"
date: 2025-09-06
weight: 1
chapter: false
pre: "<b>1.1. </b>"
---

{{% notice warning %}}
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}}

### Week 1 Objectives

* Integrate into the FCJ engineering culture and establish communication channels.
* Establish a secure **AWS Landing Zone**: Account structure, IAM Security, and Billing controls.
* **Network Deep Dive:** Master the packet flow within a Virtual Private Cloud (VPC).

### Tasks to be carried out this week

| Day | Task | Start Date | Completion Date | Reference Material |
|-----|------|------------|-----------------|---------------------|
| 2 | - **Onboarding:** Attended the Kick-off session, aligned on the training roadmap.<br>- **Team Building:** Formed the project squad and standardized collaboration tools (Discord/Slack/Trello). | 09/06/2025 | 09/06/2025 | |
| 3 | - **Environment Setup:** Provisioned the root AWS Account.<br>- **Security First:** Enforced MFA for Root User, created an IAM Admin User to avoid root access.<br>- **FinOps:** configured **AWS Budgets** to trigger alerts when costs exceed forecast. | 09/09/2025 | 09/09/2025 | [REFER HERE](https://cloudjourney.awsstudygroup.com/) |
| 4 | - **Architecture Study:** Analyzed the "3-Tier VPC Architecture" pattern via Draw.io.<br>- **AWS Support:** Researched support plans (Basic vs. Developer) and the case opening process for infrastructure incidents. | 09/10/2025 | 09/10/2025 | [REFER HERE](https://cloudjourney.awsstudygroup.com/) |
| 5 | - **VPC Implementation:**<br>&emsp;+ Initialized VPC with CIDR Block `10.0.0.0/16`.<br>&emsp;+ **Subnetting:** Segregated network into Public Subnets (Web) and Private Subnets (DB/App) for isolation.<br>&emsp;+ **Routing:** Configured Internet Gateway (IGW) and Route Tables for outbound connectivity.<br>&emsp;+ **Firewall:** Defined Security Groups to whitelist ports 22 (SSH) and 80 (HTTP). | 09/11/2025 | 09/14/2025 | [REFER HERE](https://cloudjourney.awsstudygroup.com/) |

### Week 1 Achievements

* Successfully participated in the FCJ kick-off session and connected with team members.
* Gained an understanding of the FCJ organization and its objectives.
* Successfully established a secure, cost-aware AWS environment (Landing Zone).
* Deep understanding of **VPC Isolation**: Treating the VPC as a software-defined data center.
* Differentiated traffic patterns between **Public Subnets** (IGW route attached) and **Private Subnets**.
* Mastered IP addressing strategies (CIDR) to prevent future network overlapping.