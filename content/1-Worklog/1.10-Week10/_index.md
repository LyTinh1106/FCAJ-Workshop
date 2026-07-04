---
title: "Week 10 Worklog"
date: 2026-07-03
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---



### Week 10 Objectives:

* Integrate Amazon Cognito authentication into the AWS Amplify frontend to manage user registration and login.
* Configure Amazon S3 bucket to securely store user-uploaded CV/resume files.
* Develop AWS Lambda functions to handle uploading and listing CV files from the S3 bucket.
* Establish API Gateway endpoints to integrate and secure CV management workflows from the frontend.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 8 | **Integrate Cognito into Amplify frontend and test**<br>- Integrate the AWS Amplify SDK library into the web frontend<br>- Implement sign-up, sign-in, and OTP/email verification screens utilizing Cognito User Pool<br>- Test end-to-end user authentication flows and secure routing for logged-in users only. | 21/06/2026 | 24/06/2026 | |
| 2 | **Configure S3 for CV storage**<br>- Initialize a dedicated Amazon S3 Bucket to act as the storage repository for candidate CV uploads<br>- Configure security policies (Bucket Policy) to block default public access<br>- Set up CORS configurations on S3 to enable direct file uploads from web browsers. | 22/06/2026 | 22/06/2026 | |
| 2 | **Create Lambda function to upload CV and list CVs from S3**<br>- Write Lambda function to generate S3 presigned URLs, enabling secure, direct CV uploads from the frontend<br>- Write Lambda function to list and scan existing CV files in the user's S3 folder<br>- Configure IAM policies for Lambda functions to permit S3 read and write access. | 22/06/2026 | 23/06/2026 | |
| 5 | **Create API endpoints for upload CV and list CV Lambda functions**<br>- Configure new routes on API Gateway integrating with CV upload and listing Lambda functions<br>- Integrate Cognito Authorizer on API Gateway to secure these endpoints from unauthorized calls<br>- Perform integration tests from the frontend to verify file upload and list response metadata. | 25/06/2026 | 27/06/2026 | |


### Week 10 Achievements:

* **User Authentication Integration**: Successfully integrated and tested Amazon Cognito sign-in/sign-up functionality in the Amplify frontend.
* **Document Storage Management**: Created and configured security permissions for the S3 bucket to store user CVs securely.
* **File Handling Backend Setup**: Built Lambda functions to handle CV uploading to S3 and retrieving the list of uploaded CVs.
* **Frontend-Backend API Connection**: Deployed API Gateway endpoints connecting the frontend to the backend for CV management workflows.
