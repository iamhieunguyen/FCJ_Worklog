---
title: "Worklog Week 12"
date: 2025-11-25
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---


### Week 12 Objectives: 

* **Event-Driven Architecture (EDA):** Integrate **Amazon SQS** to buffer and decouple high-volume image processing tasks.
* **Resiliency:** Implement asynchronous processing patterns to handle traffic spikes without dropping requests.
* **Production Readiness:** Finalize Domain/DNS configuration, SSL certificates, and Operational Monitoring (SNS).
* **Complete the main interfaces** of the Frontend, prepare for domain name purchase, and **attend the final AWS Cloud Mastery Series event**.

---

### Tasks to be Deployed This Week:

| Day | Task | Start Date | Completion Date | Resources |
| :--- | :--- | :--- | :--- | :--- |
| Mon | - **Feature Logic** | - Completed complex logic for `UpdateArticle` (handling concurrency and partial updates).<br>- Tuned Rekognition `MinConfidence` thresholds to improve tag relevance. | 25/11/2025 | 25/11/2025 | Application Logic |
| Tue | - **Async Pattern** | - **Architectural Upgrade:** Refactored the AI pipeline to the **Storage-First Pattern**:<br> *Upload to S3 $\rightarrow$ S3 Event $\rightarrow$ **SQS Queue** $\rightarrow$ Lambda Worker $\rightarrow$ DynamoDB*.<br>- Benefit: Provides a "buffer" to protect downstream services from throttling. |   27/11/2025 | 27/11/2025 | SQS Integration |
| Wed | **Geo-Location** | - Integrated **Map Pinning** on the frontend.<br>- Modeled geospatial data (Latitude/Longitude) in DynamoDB for future geospatial queries. | 27/11/2025 | 27/11/2025 | Feature Dev |
| Thu | - **Observability** | - Deployed **Amazon SNS** topics to alert administrators on critical system failures (CloudWatch Alarms).<br>- Audited IAM Roles to ensure "Least Privilege" before public release. | 28/11/2025 | 28/11/2025 | AWS SNS, Cognito/IAM Documentation |
| Fri | - **Go-Live Prep** | - Configured **Route 53** Alias records to point the custom domain to CloudFront (Frontend) and API Gateway (Backend).<br>- Provisioned SSL/TLS certificates via **AWS Certificate Manager (ACM)** for HTTPS security. | 29/11/2025 | 29/11/2025 | Final Polish |

---

### Week 12 Achievements: 

* **Resilient System:** The introduction of SQS created a robust Event-Driven Architecture capable of handling burst traffic without failure.
* **Enterprise Standard:** The system now features a complete serverless lifecycle: Compute (Lambda), Storage (S3), Database (DynamoDB), Integration (SQS/SNS), and Network (Route53).
* **Demo Ready:** The project is fully deployed, secured with HTTPS, and operates under a professional CI/CD and Multi-stack infrastructure.
* **Successfully participated in the final AWS Cloud Mastery Series event**, receiving comprehensive guidance for project completion.
* The project has reached **Demo Readiness** status.