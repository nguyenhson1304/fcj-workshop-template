---
title: "Week 2 Worklog"
date: 2026-10-12
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---
<!-- {{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}} -->

### Week 2 Objectives:

- Deep dive into Amazon VPC architecture (CIDR blocks, Public vs. Private Subnets, Internet Gateway, NAT Gateway)
- Understand stateful Security Groups vs. stateless Network ACLs (NACLs)
- Master Amazon EC2 lifecycle, purchasing options (On-Demand, Spot, Reserved), User Data, and Instance Roles
- Learn Elastic Load Balancing (ALB) and EC2 Auto Scaling Groups (ASG) for High Availability

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | - Study Amazon VPC fundamentals: <br>&emsp; + IPv4 CIDR block planning <br>&emsp; + Public Subnets vs. Private Subnets <br>&emsp; + Route Tables, Internet Gateways (IGW), and NAT Gateways | 12/10/2026 | 12/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 2 | - **Practice (Networking):** <br>&emsp; + Design and build a custom multi-AZ VPC from scratch <br>&emsp; + Configure public and private route tables <br>&emsp; + Configure Security Groups and NACLs | 13/10/2026 | 13/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 3 | - Study Amazon EC2 advanced concepts: <br>&emsp; + EC2 User Data bootstrapping scripts <br>&emsp; + IAM Instance Profiles (attaching IAM Roles to EC2 instead of hardcoding credentials) <br>&emsp; + AWS Systems Manager (SSM) Session Manager | 14/10/2026 | 14/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 4 | - **Practice (EC2 & IAM Role):** <br>&emsp; + Launch an EC2 instance in a private subnet <br>&emsp; + Attach an IAM Role to EC2 and access S3 via `boto3` / AWS CLI without Access Keys <br>&emsp; + Connect securely using SSM Session Manager | 15/10/2026 | 15/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 5 | - Learn High Availability & Scalability: <br>&emsp; + Application Load Balancer (ALB) & Target Groups <br>&emsp; + Launch Templates & EC2 Auto Scaling Groups (ASG) | 16/10/2026 | 16/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 6 | - **Practice (HA Architecture) & Cleanup:** <br>&emsp; + Deploy an ALB distributing HTTP traffic across EC2 instances in two Availability Zones <br>&emsp; + Verify orphan resource cleanup (EBS volumes, Elastic IPs, NAT Gateways) via Cost Explorer | 17/10/2026 | 17/10/2026 | https://cloudjourney.awsfcaj.com/ |

### Week 2 Achievements:

- Built a custom Amazon VPC with isolated public and private subnets across multiple Availability Zones.
- Understood why attaching **IAM Roles** to EC2 instances is a security best practice compared to storing static Access Keys in code[cite: 1, 2].
- Configured an Application Load Balancer (ALB) with Auto Scaling to handle traffic spikes and ensure fault tolerance.
- Practiced proper cloud hygiene by auditing and deleting unattached EBS volumes and Elastic IPs to avoid unintended `EC2-Other` charges[cite: 4].