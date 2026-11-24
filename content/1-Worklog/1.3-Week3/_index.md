---
title: "Week 3 Worklog"
date: 2026-10-19
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---
<!-- {{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}} -->

### Week 3 Objectives:

- Understand AWS Storage options: Object Storage (Amazon S3), Block Storage (Amazon EBS), and File Storage (Amazon EFS)
- Master Amazon S3 features: Storage Classes, Versioning, Lifecycle Policies, Bucket Policies, and Encryption
- Understand Relational Databases (Amazon RDS) vs. NoSQL Databases (Amazon DynamoDB)
- Deploy a full-stack web/CRUD application connecting EC2 to Amazon RDS

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | - Study Amazon S3 in depth: <br>&emsp; + Buckets, Objects, Prefixes & Partitioning <br>&emsp; + S3 Storage Classes (Standard, IA, Glacier) & Lifecycle Rules <br>&emsp; + Block Public Access, Bucket Policies & Pre-signed URLs | 19/10/2026 | 19/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 2 | - **Practice (Storage):** <br>&emsp; + Create S3 buckets, enable Versioning, and configure Lifecycle transitions <br>&emsp; + Create EBS Snapshots and test Amazon EFS shared mounting across two EC2 instances | 20/10/2026 | 20/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 3 | - Study Relational Databases (Amazon RDS & Aurora): <br>&emsp; + DB Subnet Groups, Multi-AZ vs. Read Replicas <br>&emsp; + Automated Backups & Security Group chaining | 21/10/2026 | 21/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 4 | - **Practice (EC2 + RDS Integration):** <br>&emsp; + Launch an Amazon RDS (MySQL/PostgreSQL) instance in a private subnet <br>&emsp; + Deploy a Node.js CRUD application on EC2 managed by `pm2` <br>&emsp; + Configure `.env` with the RDS endpoint and verify database connectivity | 22/10/2026 | 22/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 5 | - Study NoSQL Databases (Amazon DynamoDB) & Caching (ElastiCache): <br>&emsp; + Partition Keys, Sort Keys, GSI/LSI <br>&emsp; + Provisioned vs. On-Demand Capacity Modes & DynamoDB Streams | 23/10/2026 | 23/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 6 | - **Practice (DynamoDB):** <br>&emsp; + Create a DynamoDB table, insert/query items via AWS CLI and Python `boto3` <br>&emsp; + Clean up RDS and EC2 lab resources | 24/10/2026 | 24/10/2026 | https://cloudjourney.awsfcaj.com/ |

### Week 3 Achievements:

- Mastered Amazon S3 data lifecycle management and security controls, which serve as the foundation for cloud Data Lakes.
- Successfully deployed a Node.js CRUD application on EC2 using PM2, connected it to a private Amazon RDS instance, and resolved DNS/Security Group networking issues.
- Learned how to model NoSQL data in Amazon DynamoDB and interact with both S3 and DynamoDB programmatically using Python `boto3`.