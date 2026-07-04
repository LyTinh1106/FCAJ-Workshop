---
title: "Week 2 Worklog"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Week 2 Objectives:

* Understand the core architecture and networking concepts of Amazon Virtual Private Cloud (VPC).
* Learn how public and private subnets isolate resources while enabling controlled communication.
* Configure essential networking components, including Internet Gateway, Route Tables, and Security Groups.
* Deploy Amazon EC2 instances in both public and private subnets following AWS networking best practices.
* Understand how Elastic IP and NAT Gateway provide secure outbound internet connectivity for private resources.
* Validate connectivity between AWS resources and analyze network traffic flow within a VPC environment.
* Gain hands-on experience in designing a secure and scalable AWS network infrastructure for future cloud applications.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Lab 03 - VPC Preparation**<br>- Create VPC<br>- Configure CIDR block<br>- Create public and private subnets | 27/04/2026 | 27/04/2026 | [Lab 03: Amazon VPC and AWS Site-to-Site VPN Workshop](https://000003.awsstudygroup.com/) |
| 3 | **Configure Network Components**<br>- Create Internet Gateway<br>- Attach Internet Gateway to VPC<br>- Create Public & Private Route Tables<br>- Associate Route Tables with subnets | 28/04/2026 | 28/04/2026 | [Lab 03: Amazon VPC and AWS Site-to-Site VPN Workshop](https://000003.awsstudygroup.com/) |
| 4 | **Deploy EC2 Instances**<br>- Create Security Groups<br>- Launch EC2 instance in Public Subnet<br>- Launch EC2 instance in Private Subnet | 29/04/2026 | 29/04/2026 | [Lab 03: Amazon VPC and AWS Site-to-Site VPN Workshop](https://000003.awsstudygroup.com/) |
| 5 | **Connectivity Validation**<br>- Connect to Public EC2 via SSH<br>- Verify communication between Public and Private EC2<br>- Test internet accessibility from each subnet | 30/04/2026 | 30/04/2026 | [Lab 03: Amazon VPC and AWS Site-to-Site VPN Workshop](https://000003.awsstudygroup.com/) |
| 6 | **Enable Private Internet Access**<br>- Allocate Elastic IP<br>- Create NAT Gateway<br>- Update Private Route Table<br>- Verify outbound internet connectivity from the private EC2 instance | 01/05/2026 | 01/05/2026 | [Lab 03: Amazon VPC and AWS Site-to-Site VPN Workshop](https://000003.awsstudygroup.com/) |

### Week 2 Achievements:

* **Designed a Secure VPC Network Architecture**: Built a custom Amazon VPC with properly planned CIDR blocks, separating workloads into public and private subnets to improve security and network organization.
* **Configured Core Networking Components**: Successfully created and integrated Internet Gateway, Route Tables, and subnet associations to establish controlled inbound and outbound traffic flow.
* **Implemented Network Security Controls**: Configured Security Groups with appropriate inbound and outbound rules, ensuring that only authorized traffic could reach EC2 instances while maintaining network isolation.
* **Deployed Multi-Tier Compute Resources**: Launched Amazon EC2 instances in both public and private subnets, validating secure communication patterns between resources deployed in different network segments.
* **Enabled Secure Outbound Internet Access**: Allocated an Elastic IP, deployed a NAT Gateway, and updated private route tables to allow private EC2 instances to access software repositories and external services without exposing them to direct inbound internet traffic.
* **Validated End-to-End Connectivity**: Performed connectivity tests to verify SSH access to public instances, communication between public and private instances, and outbound internet connectivity through the NAT Gateway.
* **Strengthened AWS Networking Knowledge**: Gained practical experience in designing, configuring, troubleshooting, and validating AWS networking infrastructure, providing a solid foundation for deploying secure, highly available cloud applications in future labs.