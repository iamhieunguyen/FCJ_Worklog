---
title: "Week 8 Worklog"
date: 2025-10-28
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---


### Week 8 Objectives: 

* **Milestone:** Successfully clear the Mid-term Exam.
* **Architectural Pivot:** Transition from traditional EC2 hosting to a **Serverless** architecture (AWS Lambda, API Gateway) to reduce operational overhead.
* **AI Service Design:** Architect an asynchronous image processing pipeline using **Amazon Rekognition**.
* **Database Modeling:** Design the **DynamoDB** schema (Single Table Design vs. Multi-table) to support high-performance access patterns.
---

### Tasks to be Deployed This Week:

| Day | Task | Start Date | Completion Date | Resources |
| :--- | :--- | :--- | :--- | :--- |
| Monday | - **Milestone** | - Final review and completion of the Mid-term Competency Exam.<br>- Post-exam sprint planning with the backend team. | 10/28/2025 | 10/28/2025 | | Personal notes, AWS Builders |
| Tuesday | - **Infrastructure Setup** | - Initialized the local development environment (AWS CLI, Boto3, IDE Linting).<br>- Designed the DynamoDB `Articles` table with Partition Key (`PK`) and Sort Key (`SK`) strategies. | 10/29/2025 | 10/30/2025 |Infrastructure Setup |
| Wednesday | - **Exam Day:** Mid-term Assessment.<br>- **API Exposure** | - Configured **API Gateway** (REST API) to route HTTP requests to Lambda functions.<br>- Tested endpoints using Postman to verify payload structures. | 10/31/2025 | 10/31/2025 |   API Integration |
| Thursday | - **FaaS Development** | - Developed the first **Lambda Functions** in Python for core CRUD operations (`CreatePost`, `GetPost`).<br>- Implemented **Boto3** wrappers to interact with DynamoDB SDK. | 01/11/2025 | 01/11/2025 | Backend Dev |
| Friday | - **AI Pipeline Design** | - Designed the "Upload-Trigger" flow: User uploads image to S3 $\rightarrow$ S3 Event Notification $\rightarrow$ Lambda $\rightarrow$ AWS Rekognition.<br>- This decouples the upload latency from the processing time. | 11/02/2025 | 11/02/2025 | Event-Driven Architecture |

---

### Week 8 Achievements: 

* **Completed the mid-term exam** (October 31st).
* Successfully shifted the architectural paradigm to Serverless, eliminating the need for OS patching and server management.
* Established the foundational API pipeline: **Client $\rightarrow$ API Gateway $\rightarrow$ Lambda $\rightarrow$ DynamoDB**.
* Defined a scalable strategy for AI integration using event triggers rather than synchronous API calls.
* Architected a scalable, asynchronous **AI Processing Pipeline**, decoupling user uploads from heavy image processing tasks (Event-driven).