---
title: "Worklog Week 9"
date: 2025-11-04
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---


### Week 9 Objectives: 

* **Infrastructure as Code (IaC):** Codify all manual resources using **AWS SAM (Serverless Application Model)** to ensure reproducibility.
* **Environment Consistency:** Eliminate "works on my machine" issues by containerizing the build process with **Docker**.
* **Deployment Strategy:** Establish a reliable "Cloud-based Development" workflow to validate IAM permissions and service integrations.
* Integrate **Docker** to standardize the environment for `sam build`.

---

### Tasks to be Deployed This Week:

| Day | Task | Start Date | Completion Date | Resources |
| :--- | :--- | :--- | :--- | :--- |
| Monday | - **IaC Definition** | - Authored the `template.yaml` to define Serverless resources (Functions, APIs, Tables).<br>- Applied **SAM Policy Templates** (e.g., `DynamoDBCrudPolicy`) to enforce the Principle of Least Privilege. | 04/11/2025 | 04/11/2025 | CloudFormation |
| Tuesday | - **Containerization** | - Integrated **Docker** into the `sam build --use-container` workflow.<br>- Solved binary incompatibility issues (Python libraries with C-extensions) between local Windows/Mac OS and the AWS Lambda Linux environment. | 05/11/2025 | 06/11/2025 | Build Runtime |
| Wednesday | - **Troubleshooting** | - Encountered limitations with `sam local start-api` (local emulation does not support full IAM or Service integration).<br>- Root caused build failures related to `requirements.txt` dependency conflicts. | 06/11/2025 | 07/11/2025 | Debugging |
| Thursday | - **Strategy Shift** | - Transitioned from Local Emulation to **Cloud-based Testing**.<br>- Provisioned a dedicated `dev` stack on AWS to run integration tests against real service endpoints. | 07/11/2025 | 08/11/2025 |   Shift-Right Testing |
| Friday | - **First Deployment** | - Successfully executed `sam deploy --guided` to the development environment.<br>- Verified the CloudFormation Stack creation and resource output values. | 08/11/2025 | 08/11/2025 | Deployment |

---

### Week 9 Achievements: 

* **Completed the technology transition** to the **AWS SAM** development model for the entire project.
* **Infrastructure is now Code:** The entire environment can be spun up or torn down with a single CLI command (`sam deploy`/`sam delete`).
* **Consistent Runtimes:** Docker integration ensures that code compiled locally runs identically in production.
* **Testing Maturity:** Moved to a more reliable testing strategy that validates actual AWS cloud behaviors and permissions.