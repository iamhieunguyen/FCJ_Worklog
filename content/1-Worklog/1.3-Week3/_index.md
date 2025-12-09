---
title: "Week 3 Worklog"
date: 2025-09-21
weight: 3
chapter: false
pre: "<b>1.3. </b>"
---


### Week 3 Objectives

* Solve the **Hybrid DNS** resolution challenge between On-premise and Cloud environments.
* Implement Cross-VPC connectivity using **VPC Peering**.
* Infrastructure troubleshooting and account stabilization.
* Discuss project plans and programming language choices with the team.

### Tasks to be carried out this week

| Day | Task | Start Date | Completion Date | Reference Material |
|-----|------|------------|-----------------|---------------------|
| 2 | - **Account Recovery:** Resolved billing/payment method issues to ensure business continuity for the training environment. | 09/21/2025 | 09/23/2025 | [REFER HERE](https://aws.amazon.com/getting-started/) |
| 3 | - **Route 53 Resolver:**<br>&emsp;+ **Inbound Endpoint:** Enabling On-prem to resolve Cloud domains.<br>&emsp;+ **Outbound Endpoint:** Enabling Cloud resources to resolve On-prem domains.<br>- Executed DNS Forwarding labs. | 09/24/2025 | 09/25/2025 | [REFER HERE](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 4 | - **VPC Peering Setup:**<br>&emsp;+ Established peering between two distinct VPCs.<br>&emsp;+ **Routing:** Updated Route Tables in both VPCs to direct traffic via the Peering Connection (`pcx-xxx`).<br>&emsp;+ Verified connectivity using private IPs. | 09/25/2025 | 09/26/2025 | [REFER HERE](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 5 | - **Project Planning:** Initial brainstorming session for the Capstone Project based on learned core services. | 09/28/2025 | 09/28/2025 | |

### Week 3 Achievements

- Successfully created a new AWS account with initial configurations, ensuring continued participation with the FCJ team.
- Gained a solid understanding of Route 53 and Hybrid DNS configuration:
  - Created and configured Outbound Endpoint for Route 53 Resolver.
  - Set up Route 53 Resolver and Inbound Endpoints.
  - Successfully connected to RD Gateway Server during practical exercises.
* Mastered **Route 53 Resolver** architecture for complex Hybrid Cloud DNS scenarios.
* Understood **VPC Peering** limitations:
    * Non-transitive nature (VPC A <-> B <-> C does not imply A <-> C).
    * Requirement for "DNS Resolution" enabling to resolve private hostnames.
* Stabilized the sandbox environment for advanced networking labs.