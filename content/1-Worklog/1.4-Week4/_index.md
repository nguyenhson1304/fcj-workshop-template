---
title: "Week 4 Worklog"
date: 2026-10-26
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---
<!-- {{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}} -->

### Week 4 Objectives:

- Master AWS IAM Least Privilege policies, AWS KMS encryption, and AWS Secrets Manager
- Configure VPC Endpoints for private AWS service access without traversing the public internet
- Understand Serverless computing with AWS Lambda, Amazon API Gateway, and event-driven messaging (SQS, SNS, Step Functions)

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | - Deep dive into AWS IAM & Cryptography: <br>&emsp; + Least Privilege JSON Policies & IAM Policy Simulator <br>&emsp; + AWS KMS (Customer Managed Keys, SSE-KMS) & AWS Secrets Manager | 26/10/2026 | 26/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 2 | - **Practice (Security & VPC Endpoints):** <br>&emsp; + Store credentials in Secrets Manager and retrieve them via Python `boto3` <br>&emsp; + Configure an S3 Gateway VPC Endpoint for private subnet access | 27/10/2026 | 27/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 3 | - Study AWS Lambda & Amazon API Gateway: <br>&emsp; + Lambda Execution Roles, Layers, Cold Starts, and Event Sources <br>&emsp; + API Gateway REST/HTTP APIs & Lambda Proxy Integration | 28/10/2026 | 28/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 4 | - **Practice (Event-Driven Lambda):** <br>&emsp; + Create a Python Lambda function triggered automatically on S3 object upload (`s3:ObjectCreated:*`) <br>&emsp; + Package dependencies using Lambda Layers | 29/10/2026 | 29/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 5 | - Study Decoupled Messaging & Orchestration: <br>&emsp; + Amazon SQS (Queues & Dead-Letter Queues) & Amazon SNS (Pub/Sub) <br>&emsp; + AWS Step Functions for multi-step serverless workflows | 30/10/2026 | 30/10/2026 | https://cloudjourney.awsfcaj.com/ |
| 6 | - **Practice (Serverless Workflow):** <br>&emsp; + Build an SNS -> SQS -> Lambda pipeline with a Dead-Letter Queue (DLQ) <br>&emsp; + Orchestrate sequential Lambda tasks in AWS Step Functions | 31/10/2026 | 31/10/2026 | https://cloudjourney.awsfcaj.com/ |

### Week 4 Achievements:

- Applied the Principle of Least Privilege in IAM and eliminated hardcoded secrets using AWS Secrets Manager and KMS.
- Built event-driven serverless functions in AWS Lambda triggered directly by S3 events.
- Designed decoupled, fault-tolerant workflows using SQS Dead-Letter Queues and AWS Step Functions.