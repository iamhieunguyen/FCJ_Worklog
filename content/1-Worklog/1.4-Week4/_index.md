---
title: "Week 4 Worklog"
date: 2025-09-29
weight: 4
chapter: false
pre: "<b>1.4. </b>"
---


### Week 4 Objectives

- Transition from Peering to **AWS Transit Gateway (TGW)** for scalable networking.
- Deep dive into EC2 optimization (Auto Scaling, Purchasing Options).
- Standardize the development workflow with **Git/GitHub**.

### Tasks to be carried out this week

| Day | Task | Start Date | Completion Date | Reference Material |
|-----|------|------------|-----------------|---------------------|
| 2 | - **Advanced Networking:** Deployed **Transit Gateway**.<br>- **Architectural Analysis:** TGW (Hub-and-Spoke) vs. Peering (Mesh). Validated TGW's efficiency in simplifying routing tables for multi-VPC environments. | 09/29/2025 | 09/30/2025 | [REFER HERE](https://aws.amazon.com/transit-gateway/) |
| 3 | - **EC2 Optimization:**<br>&emsp;+ **Auto Scaling Group (ASG):** Implemented dynamic scaling policies based on CPU utilization.<br>&emsp;+ **Cost Strategy:** Analyzed Spot Instances (90% savings) vs. Reserved/Savings Plans. | 10/01/2025 | 10/02/2025 | [REFER HERE](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 4 | - **Source Control Governance:**<br>&emsp;+ Enforced Git practices: `git clone`, `branching strategies`, `PR reviews`.<br>&emsp;+ Resolved merge conflicts in collaborative scenarios. | 10/03/2025 | 10/04/2025 | [REFER HERE](https://www.youtube.com/watch?v=8O14qT3jdq0&list=PLodO7Gi1F7R0t9SyEZF5mwfKevCULLjgG&index=2) |
| 5 | - **Pre-Proposal:** Brainstormed project feasibility, tech stack selection, and module division (BE/FE/DevOps). | 10/05/2025 | 10/06/2025 | |

### Week 4 Achievements

- Mastered the setup and configuration of AWS Transit Gateway, understanding its advantages over VPC Peering (e.g., support for complex multi-VPC and resource connections).
- Gained a solid understanding of Amazon EC2’s key features:
  - Flexible instance configurations.
  - Cost optimization through various pricing models.
* Recognized **Transit Gateway** as the enterprise standard for centralizing network connectivity, eliminating the complexity of managing N*(N-1)/2 peering connections.
* Defined a compute strategy: **Spot Instances** for stateless/fault-tolerant workloads, **Reserved** for steady-state databases.
* Established a clean **Git Flow**, readying the team for parallel development.