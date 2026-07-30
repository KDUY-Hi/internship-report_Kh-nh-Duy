---
title: "Week 4 - AWS Architecture, IAM, and Security Groups"
date: 2026-06-29
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Goals

- Study the AWS deployment architecture for the project.
- Understand the roles of IAM, VPC, subnets, and Security Groups.
- Define how the frontend, backend, database, and storage components should be separated in the cloud environment.

### Work Completed

| Day | Task | Start Date | Completion Date | Reference |
| --- | --- | --- | --- | --- |
| Day 1 | Analyze the overall cloud architecture<br>Identify which AWS services should host the frontend, backend, database, and file storage | 2026-06-29 | 2026-06-29 | AWS Architecture Center / AWS Docs |
| Day 2 | Study IAM and the principle of least privilege<br>Distinguish IAM Users, IAM Roles, policies, and service access permissions | 2026-06-30 | 2026-06-30 | IAM Docs / AWS Security Best Practices |
| Day 3 | Study VPC, subnets, and basic routing<br>Understand public subnets, private subnets, and safer database placement | 2026-07-01 | 2026-07-01 | Amazon VPC Docs |
| Day 4 | Design Security Groups for the project<br>Restrict SSH, open only required HTTP/HTTPS/API ports, and allow database access only from the backend | 2026-07-02 | 2026-07-02 | Security Group Docs / AWS Well-Architected |

### Results

The team defined an initial AWS architecture for the project and understood how to control access between components. This was an important preparation step before creating real resources such as S3, EC2, and RDS in the following weeks.
