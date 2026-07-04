---
title: "Week 3 Worklog"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

* Understand hybrid DNS architecture using Amazon Route 53 Resolver.
* Learn how Route 53 Inbound and Outbound Resolver Endpoints enable DNS communication between AWS and on-premises environments.
* Deploy and configure Microsoft Active Directory (AD) infrastructure for hybrid networking scenarios.
* Gain hands-on experience with AWS CloudFormation to automate infrastructure deployment.
* Understand the architecture and use cases of VPC Peering for private communication between isolated VPCs.
* Configure routing, Network ACLs, Security Groups, and Cross-Peer DNS resolution to enable secure inter-VPC connectivity.
* Validate DNS resolution and network communication across hybrid and peered network environments.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
|2 | **Lab 10 - Set up Hybrid DNS with Route 53 Resolver**<br>- Environment Preparation <br>- Generate key pair<br>- Initialize CloudFormation template<br>- Configure Security Groups | 04/05/2026 | 04/05/2026 | [Lab 10: Set up Hybrid DNS with Route 53 Resolver](https://000010.awsstudygroup.com/) |
| 3 | **Deploy Hybrid DNS Infrastructure**<br>- Connect to Remote Desktop Gateway (RDGW)<br>- Deploy Microsoft Active Directory<br>- Verify Active Directory environment | 05/05/2026 | 05/05/2026 | [Lab 10: Set up Hybrid DNS with Route 53 Resolver](https://000010.awsstudygroup.com/) |
| 4 | **Configure Route 53 Resolver**<br>- Create Route 53 Outbound Endpoint<br>- Create Route 53 Resolver Rules<br>- Create Route 53 Inbound Endpoint<br>- Validate DNS resolution | 06/05/2026 | 06/05/2026 | [Lab 10: Set up Hybrid DNS with Route 53 Resolver](https://000010.awsstudygroup.com/) |
| 5 | **Lab 19 - VPC Peering Preparation**<br>- Deploy CloudFormation stacks (my-vpc & hg-vpc)<br>- Create Security Groups<br>- Launch EC2 instances in both VPCs | 07/05/2026 | 07/05/2026 | [Lab 19: VPC Peering](https://000019.awsstudygroup.com/) |
| 6 | **Configure VPC Peering**<br>- Create VPC Peering Connection<br>- Update Route Tables<br>- Modify Network ACLs | 08/05/2026 | 08/05/2026 | [Lab 19: VPC Peering](https://000019.awsstudygroup.com/) |
| 7 | **Validate Inter-VPC Connectivity**<br>- Enable Cross-Peer DNS Resolution<br>- Test connectivity between EC2 instances across VPCs<br>- Verify private DNS name resolution | 09/05/2026 | 09/05/2026 | [Lab 19: VPC Peering](https://000019.awsstudygroup.com/) |

### Week 3 Achievements:

* **Built a Hybrid DNS Infrastructure**: Configured Amazon Route 53 Resolver with Inbound and Outbound Endpoints, enabling seamless DNS resolution between AWS resources and an on-premises Microsoft Active Directory environment.
* **Automated Infrastructure Deployment**: Leveraged AWS CloudFormation templates to provision networking resources and supporting infrastructure, reducing manual configuration and improving deployment consistency.
* **Integrated Microsoft Active Directory with AWS**: Successfully deployed and configured Microsoft Active Directory alongside a Remote Desktop Gateway (RDGW), establishing the foundation for hybrid identity and DNS services.
* **Implemented Secure Hybrid Name Resolution**: Created Route 53 Resolver Rules to forward DNS queries between AWS and on-premises networks, validating bidirectional domain name resolution.
* **Established Private Inter-VPC Connectivity**: Configured VPC Peering between two independent VPCs, allowing direct private communication without traversing the public internet.
* **Configured Network Routing and Security**: Updated Route Tables, Network ACLs, and Security Groups to securely route traffic across peered VPCs while maintaining proper network isolation.
* **Enabled Cross-Peer DNS Resolution**: Configured DNS resolution across peered VPCs, allowing EC2 instances to communicate using private DNS hostnames instead of IP addresses.
* **Strengthened AWS Networking Expertise**: Gained practical experience in designing hybrid networking solutions, automating infrastructure deployment, and implementing secure private connectivity between AWS environments.