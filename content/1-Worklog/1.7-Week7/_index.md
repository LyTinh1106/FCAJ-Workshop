---
title: "Week 7 Worklog"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:

* Master AWS Identity and Access Management (IAM) advanced access control using Resource Tags and Policies.
* Configure IAM Role Conditions to restrict role-assumption by specific IP and Time constraints.
* Authorize applications on Amazon EC2 to securely access Amazon S3 buckets using IAM Roles.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Lab 28: Manage Access to EC2 Services with Resource Tags through IAM Services** <br>- Create new IAM user for the lab <br>- Create custom IAM policy and IAM role <br>- Verify policy application on the IAM user: <br>&emsp; + Switch role <br>&emsp; + Test regional EC2 console access: Tokyo (denied) vs. N. Virginia (allowed) <br>&emsp; + Verify EC2 creation rules (without tags vs. with conforming tags) <br>&emsp; + Test editing Resource Tags on EC2 instance (denied by policy) | 01/06/2026 | 01/06/2026      | [Lab 28: Manage Access to EC2 Services with Resource Tags through IAM Services](https://000028.awsstudygroup.com/) |
| 3 | **Lab 44: IAM Role & Condition** <br>- Create IAM group and IAM users <br>- Verify default user permissions <br>- Configure IAM Admin Role and switch role parameters <br>- Apply conditions to restrict switch role permissions: <br>&emsp; + Limit role switching by specific IP address <br>&emsp; + Limit role switching by specific time window | 02/06/2026 | 02/06/2026      | [Lab 44: IAM Role & Condition](https://000044.awsstudygroup.com/) |
| 4 | **Lab 48: Granting Authorization for Application to Access AWS Services with IAM Role** <br>- Deploy environment: launch an EC2 instance and create an S3 bucket <br>- Create a specific IAM user and activate an access key <br>- Create an IAM role to grant secure S3 access using temporary credentials via the access key | 04/06/2026 | 04/06/2026      | [Lab 48: Granting Authorization for Application to Access AWS Services with IAM Role](https://000048.awsstudygroup.com/) |


### Week 7 Achievements:

* **Implemented Attribute-Based Access Control (ABAC)**: Enforced strict access boundaries on EC2 instances by utilizing IAM policy condition keys matched with resource tags.
* **Controlled Region-Level Access**: Verified IAM policies restricting service control interfaces across regions, validating successful operations in `us-east-1` (North Virginia) while blocking access in `ap-northeast-1` (Tokyo).
* **Applied Advanced IAM Policy Conditions**: Restricted administrative role-assumption privileges by incorporating multi-factor conditional rules (IP address constraints and specific time-window execution limits).
* **Managed App-to-Service Authorization**: Enabled secure and standard programmatic access to S3 resources from compute nodes without embedding static secret credentials directly onto code or instances.
