---
title: "Worklog Week 11"
date: 2024-11-18
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---


### Week 11 Objectives: 

* **Participate in AWS Cloud Mastery Series #2** to continue resolving specialized technical issues.
* **Architecture Refactoring:** Decompose the monolithic `template.yaml` into a **Multi-Stack** architecture (Nested Stacks) to reduce "Blast Radius" and improve deployment speed.
* **Dependency Optimization:** Implement **Lambda Layers** to share common code and reduce deployment package size.
* **Pipeline Stability:** Fix circular dependencies and export/import errors in CloudFormation.
---

### Tasks to be Deployed This Week:

| Day | Task | Start Date | Completion Date | Resources |
| :--- | :--- | :--- | :--- | :--- |
| Sun | - **Participate in AWS Cloud Mastery Series #2 (Nov 17th):** - Researched "Strangler Fig" and "Fan-out" patterns from AWS Cloud Mastery resources to apply to the refactoring process. | 17/11/2024 | 17/11/2024 | Mentor, AWS Cloud Mastery Series |
| Mon | - **Stack Strategy** | - Split the monolith into logical stacks:<br> 1. **Core-Infra:** VPC, Security Groups (Stable/Static).<br> 2. **Data-Stack:** DynamoDB, S3 Buckets (Stateful).<br> 3. **App-Stack:** Lambda, API Gateway (Stateless/High Churn). | 18/11/2024 | 18/11/2024 | IaC Modularization |
| Tue | - **Pipeline Fixes** | - **Critical Bug:** Hit a "Circular Dependency" error where Stack A referenced Stack B, and B referenced A.<br>- **Fix:** Refactored parameter passing and removed bidirectional references by using SSM Parameter Store for runtime configuration. | | 19/11/2024 | 19/11/2024 | Troubleshooting |
| Wed | - Extracted heavy libraries (`boto3`, `requests`, `Pillow`) into a shared **Lambda Layer**.<br>- Result: Reduced individual function code size from 10MB to <50KB, significantly improving cold start times. | 20/11/2024 | 20/11/2024 | Optimization |
| Thu | - **Stabilization** | - Finalized the deployment script (`deploy.sh`) to orchestrate the stack creation order.<br>- Synced the Frontend codebase to align with the new API Gateway IDs. | | 21/11/2024 | 21/11/2024 | API Gateway/Lambda Configuration |
| Fri | - **Team Meeting and Project Stabilization:** Held a team meeting to review the new Frontend structure, stabilize the main project Stack, and synchronize the fixes for CORS and basic template errors. <br> - **Cross-Stack Refs** | - Utilized `AWS::CloudFormation::Stack` to nest templates.<br>- Configured `Outputs` and `Fn::ImportValue` to pass resource IDs | 22/11/2024 | 22/11/2024 | Stack Dependencies |

---

### Week 11 Achievements: 

* **Participated in AWS Cloud Mastery Series #2**, gaining deeper knowledge of Serverless, Rekognition, and solutions for authorization errors.
* Successfully migrated to a **Multi-Stack Architecture**, isolating stateful resources (DB) from stateless code (Lambda). This prevents accidental database deletion during code updates.
* Reduced deployment time by allowing independent updates to the Application Stack.
* Eliminated code duplication across functions using Lambda Layers.
* **Developed a separate stack for backup/optimization**, enhancing project flexibility and safety during future major updates.