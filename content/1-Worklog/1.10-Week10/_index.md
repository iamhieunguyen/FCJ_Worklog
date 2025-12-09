---
title: "Worklog Week 10"
date: 2025-11-11
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Week 10 Objectives: 

* **Stabilize the AWS SAM/Serverless deployment environment.**
* **Network Security:** Implement rigid **CORS (Cross-Origin Resource Sharing)** policies to secure browser-based API calls.
* **Authentication:** Integrate **Amazon Cognito** for centralized user identity management and secure API access.
* **Frontend-Backend Wiring:** Connect the React Frontend to the Serverless Backend and troubleshoot integration friction.
* **Participate in the AWS Cloud Mastery Series event** to receive guidance and address project inquiries.

---

### Tasks to be Deployed This Week:

| Day | Task | Start Date | Completion Date | Resources |
| :--- | :--- | :--- | :--- | :--- |
| Mon | - **CORS Engineering** | - Configured API Gateway OPTIONS methods and Lambda response headers (`Access-Control-Allow-Origin`).<br>- Debugged "Preflight Request" failures in the browser console. | 11/11/2025 | 11/11/2025 | API Gateway Config |
| Tue | - **Data Optimization** | - Optimized DynamoDB access patterns using **GSI (Global Secondary Indexes)** to support "Get All Articles" queries efficiently.<br>- Standardized API response payloads to JSON API specifications. | 12/11/2025 | 12/11/2025 | Database Tuning  |
| Wed | - **Frontend Integration** | - Deployed Frontend assets to S3 Static Website Hosting.<br>- Injected API endpoints via Environment Variables during the frontend build process. | 13/11/2025 | 13/11/2025 | CI/CD Prep |
| Thu | - **Identity & Access** | - Configured **Cognito User Pool** and connected it to API Gateway Authorizers.<br>- **Bug Fix:** Debugged a `Sub ID` mismatch where the Lambda function failed to map the Cognito Token ID to the user profile in DynamoDB. | 14/11/2025 | 14/11/2025 | Auth/Authz   |
| Fri | - **Participation in AWS Cloud Mastery Series:** <br>&emsp; + Received guidance and clarified questions regarding Serverless, Rekognition. <br> - **Analyze Update/Rekognition error:** Begin applying mentor guidance to resolve authorization issues and Rekognition-related errors. | 15/11/2025 | 15/11/2025 | Mentor, AWS Cloud Mastery Series |

---

### Week 10 Achievements: 

* **Participated in the AWS Cloud Mastery Series event** and gathered necessary information to solve major project bugs.
* Resolved critical **CORS issues**, enabling secure communication between the web client and the API.
* Implemented **Token-based Authentication** (JWT), ensuring that only authenticated users can access modify/delete endpoints.
* Validated the end-to-end flow: Login $\rightarrow$ Get Token $\rightarrow$ Call API $\rightarrow$ Update DB.
* The project has transitioned to the basic user testing phase.

---