---
title: "Week 9 Worklog"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---


### Week 9 Objectives:

* Build an automated system to fetch job data via API using Amazon EventBridge/Scheduler.
* Deploy and host the web application frontend on AWS Amplify.
* Design a DynamoDB database and build AWS Lambda functions to process and store job information.
* Configure API Gateway to serve as a secure entry point for backend services.
* Securely manage API Keys and secrets using AWS Systems Manager Parameter Store.
* Learn about Amazon Cognito identity management and configure Cognito User Pool.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | **Create schedule to automatically fetch API**<br>- Research and learn about Amazon EventBridge (Scheduler)<br>- Set up rules and cron expression schedules to run periodically daily to automatically trigger APIs for fetching latest Job data<br>- Verify execution logs to ensure the scheduler triggers accurately on time. | 15/06/2026 | 15/06/2026 | |
| 3 | **Host frontend using Amplify**<br>- Configure the frontend project on the AWS Amplify Console<br>- Connect the frontend source code repository (GitHub/GitLab)<br>- Set up CI/CD pipelines to automatically build and deploy upon repository changes<br>- Configure domain routing and verify application accessibility. | 16/06/2026 | 16/06/2026 | |
| 5 | **Build Lambda Function and DynamoDB Table to store Jobs**<br>- Design the DynamoDB schema for storing Job details, defining appropriate Partition Key and Sort Key<br>- Write Lambda function code (Python/Node.js) to format API payload and write it into DynamoDB<br>- Configure IAM Role and policies to grant the Lambda function write permissions to DynamoDB. | 18/06/2026 | 18/06/2026 | |
| 6 | **Configure API Gateway**<br>- Initialize a REST API or HTTP API on Amazon API Gateway<br>- Configure resources and methods (e.g., POST, GET) integrating directly with the Lambda backend<br>- Configure CORS to allow secure API calls from the frontend application<br>- Deploy the API to a stage and test endpoint connectivity. | 19/06/2026 | 19/06/2026 | |
| 6 | **Configure Parameter Store to store API Keys**<br>- Use AWS Systems Manager Parameter Store to securely store sensitive configurations and API Keys<br>- Assign IAM policies to the Lambda Function to securely read keys from the Parameter Store<br>- Update Lambda source code to dynamically retrieve API Keys from the Parameter Store instead of hardcoding. | 19/06/2026 | 19/06/2026 | |
| 7 | **Learn about Cognito and configure Cognito User Pool**<br>- Research Amazon Cognito architecture and user management features<br>- Initialize Cognito User Pool and set up required user attributes (email, password policy)<br>- Configure App Client and define authentication flows (OAuth, hosted UI). | 20/06/2026 | 20/06/2026 | |


### Week 9 Achievements:

* **Data Fetching Automation**: Successfully set up an automated schedule to periodically fetch API data.
* **Frontend Web Deployment**: Successfully hosted the application frontend on AWS Amplify with global accessibility.
* **Serverless Backend & Database**: Built a complete Lambda function and DynamoDB table to reliably and efficiently store job data.
* **Secure API Gateway Management**: Configured API Gateway endpoints to allow the frontend to interact with the Lambda backend.
* **Secrets Security**: Securely stored sensitive API keys and configuration settings using Parameter Store, enhancing system security.
* **Identity Workflow Setup**: Configured Cognito User Pool, ready for integrating user registration and login features.
