---
title: "Week 5 - Preparing S3, RDS, and EC2"
date: 2026-07-06
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Goals

- Prepare the core AWS services required by the project.
- Design CV storage using a private S3 bucket.
- Plan the backend deployment on EC2 and the production database on RDS PostgreSQL.

### Work Completed

| Day | Task | Start Date | Completion Date | Reference |
| --- | --- | --- | --- | --- |
| Day 1 | Study Amazon S3 for file storage<br>Design a private bucket for CV files and avoid exposing sensitive data publicly | 2026-07-06 | 2026-07-06 | Amazon S3 Docs |
| Day 2 | Study Amazon RDS PostgreSQL<br>Define the production database, subnet, Security Group, and migration process | 2026-07-07 | 2026-07-07 | Amazon RDS Docs / PostgreSQL Docs |
| Day 3 | Study Amazon EC2 for the backend<br>Prepare the model for running FastAPI with Uvicorn on a Linux server | 2026-07-08 | 2026-07-08 | Amazon EC2 Docs / FastAPI Docs |
| Day 4 | Create an AWS deployment checklist<br>Summarize environment variables, secrets, inbound rules, CORS, and post-deployment tests | 2026-07-09 | 2026-07-09 | AWS Docs / Project checklist |

### Results

The team had a clearer AWS deployment plan before starting real configuration. S3, RDS, and EC2 were assigned specific roles in the project architecture.
