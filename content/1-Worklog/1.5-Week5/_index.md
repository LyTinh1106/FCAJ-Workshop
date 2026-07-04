---
title: "Week 5 Worklog"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Understand how AWS Lambda can automate operational tasks to reduce Amazon EC2 running costs.
* Learn to implement resource management using AWS Lambda and Amazon EC2 APIs.
* Configure IAM Roles with least-privilege permissions to enable secure Lambda execution.
* Deploy a supporting VPC environment and configure Security Groups for EC2 instances.
* Integrate AWS Lambda with Slack using Incoming Webhooks to receive real-time infrastructure notifications.
* Implement tag-based automation to selectively manage EC2 instances without affecting other resources.
* Validate automated instance lifecycle management and monitor execution through AWS CloudWatch logs and Slack notifications.
* Gain practical experience in building event-driven automation solutions that improve operational efficiency and cost optimization.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2| **Lab 22 - Optimizing EC2 Costs with Lambda** <br>- Environment Prepairation <br>- Create VPC<br>- Enable Auto-assign Public IPv4 Address for public subnets<br>- Create Security Group | 18/05/2026 | 18/05/2026 | [Lab 22: Optimizing EC2 Costs with Lambda](https://000022.awsstudygroup.com/) |
| 3 | **Deploy Compute Resources**<br>- Launch EC2 instance<br>- Configure EC2 instance tags for automation<br>- Create Slack Workspace and Incoming Webhook | 19/05/2026 | 19/05/2026 | [Lab 22: Optimizing EC2 Costs with Lambda](https://000022.awsstudygroup.com/) |
| 4 | **Configure IAM and Lambda**<br>- Create IAM Role for Lambda execution<br>- Assign permissions to manage EC2 instances<br>- Verify IAM Role configuration | 20/05/2026 | 20/05/2026 | [Lab 22: Optimizing EC2 Costs with Lambda](https://000022.awsstudygroup.com/) |
| 5 | **Develop Automation Functions**<br>- Create Lambda function to stop EC2 instances<br>- Create Lambda function to start EC2 instances<br>- Integrate Slack notification logic | 21/05/2026 | 21/05/2026 | [Lab 22: Optimizing EC2 Costs with Lambda](https://000022.awsstudygroup.com/) |
| 6 | **Validate Automation Workflow**<br>- Test automatic start and stop operations<br>- Verify Lambda execution logs<br>- Confirm Slack notifications and EC2 state transitions | 22/05/2026 | 22/05/2026 | [Lab 22: Optimizing EC2 Costs with Lambda](https://000022.awsstudygroup.com/) |

### Week 5 Achievements:

* **Automated EC2 Cost Optimization**: Developed AWS Lambda functions to automatically start and stop Amazon EC2 instances based on operational requirements, reducing unnecessary compute costs for non-production workloads.
* **Implemented Tag-Based Resource Management**: Applied EC2 instance tags to identify automation targets, enabling scalable and selective resource management without impacting unrelated infrastructure.
* **Configured Secure Serverless Permissions**: Created IAM Roles following the Principle of Least Privilege, allowing Lambda functions to securely manage EC2 instances while minimizing unnecessary permissions.
* **Built an Event-Driven Automation Workflow**: Designed a serverless automation solution that integrates AWS Lambda with Amazon EC2 APIs to perform infrastructure operations without manual intervention.
* **Integrated Real-Time Operational Notifications**: Connected AWS Lambda with Slack using Incoming Webhooks, automatically delivering notifications whenever EC2 instances were started or stopped.
* **Validated End-to-End Automation**: Successfully tested the complete automation workflow by verifying EC2 state transitions, reviewing CloudWatch execution logs, and confirming Slack notification delivery.
* **Strengthened Cloud Operations Skills**: Gained practical experience in serverless computing, infrastructure automation, IAM security, and operational cost optimization using AWS-native services and event-driven architectures.