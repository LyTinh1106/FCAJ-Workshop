---
title: "Week 4 Worklog"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:

* Understand the architecture and use cases of AWS Transit Gateway for connecting multiple Virtual Private Clouds (VPCs).
* Learn how Transit Gateway simplifies network topology compared to VPC Peering in large-scale AWS environments.
* Configure Transit Gateway attachments and route tables to enable controlled communication between multiple VPCs.
* Validate end-to-end connectivity across interconnected VPCs using centralized routing.
* Understand the core concepts of AWS Backup, including Backup Plans, Backup Vaults, lifecycle policies, and recovery points.
* Configure automated backup schedules and notification mechanisms to improve data protection.
* Perform backup restoration and verify data integrity as part of disaster recovery testing.
* Gain practical experience in designing resilient networking and backup strategies following AWS best practices.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Lab 20 - Transit Gateway**<br>- Generate key pair (`tgw-key`)<br>- Initialize CloudFormation template<br>- Deploy networking infrastructure | 11/05/2026 | 11/05/2026 | [Lab 20: Transit Gateway](https://000020.awsstudygroup.com/) |
| 3 | **Configure Transit Gateway**<br>- Create Transit Gateway<br>- Create Transit Gateway Attachments for VPC2, VPC3, and VPC4<br>- Verify attachment status | 12/05/2026 | 12/05/2026 | [Lab 20: Transit Gateway](https://000020.awsstudygroup.com/) |
| 4 | **Configure Network Routing**<br>- Create Transit Gateway Route Table<br>- Update VPC Route Tables for all connected VPCs<br>- Test inter-VPC connectivity | 13/05/2026 | 13/05/2026 | [Lab 20: Transit Gateway](https://000020.awsstudygroup.com/) |
| 5 | **Lab 13 - AWS Backup**<br>- Create Amazon S3 bucket<br>- Deploy backup infrastructure<br>- Verify required resources | 14/05/2026 | 14/05/2026 | [Lab 13: AWS Backup](https://000013.awsstudygroup.com/) |
| 6 | **Configure AWS Backup**<br>- Create Backup Plan<br>- Configure backup rules and lifecycle policies<br>- Configure backup notifications | 15/05/2026 | 15/05/2026 | [Lab 13: AWS Backup](https://000013.awsstudygroup.com/) |
| 7 | **Validate Backup and Recovery**<br>- Execute backup jobs<br>- Restore protected resources<br>- Verify restoration results and backup integrity | 16/05/2026 | 16/05/2026 | [Lab 13: AWS Backup](https://000013.awsstudygroup.com/) |

### Week 4 Achievements:

* **Designed a Hub-and-Spoke Network Architecture**: Deployed AWS Transit Gateway as a centralized routing hub connecting multiple VPCs, reducing network complexity and providing a scalable alternative to managing numerous VPC Peering connections.
* **Implemented Centralized Inter-VPC Routing**: Configured Transit Gateway Attachments and Transit Gateway Route Tables, enabling controlled communication between multiple VPCs while maintaining simplified route management.
* **Validated Secure Multi-VPC Connectivity**: Updated VPC Route Tables and verified end-to-end communication between EC2 instances across connected VPCs, ensuring traffic remained within the AWS private network.
* **Built an Automated Backup Strategy**: Configured AWS Backup by creating Backup Plans with scheduled backup rules, retention policies, and lifecycle configurations to automate data protection.
* **Configured Backup Monitoring and Notifications**: Enabled backup notifications to monitor backup job execution, improving operational visibility and ensuring backup tasks completed successfully.
* **Verified Disaster Recovery Procedures**: Performed backup restoration tests to validate recovery points, confirm data integrity, and ensure workloads could be successfully restored during recovery scenarios.
* **Strengthened Infrastructure Resilience**: Gained practical experience in implementing highly available network connectivity and automated backup solutions, establishing a strong foundation for secure, scalable, and disaster-resilient AWS environments.