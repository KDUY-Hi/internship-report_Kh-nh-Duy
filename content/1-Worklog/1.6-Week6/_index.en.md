---
title: "Week 6 - S3 and Backend Deployment on EC2"
date: 2026-07-13
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Goals

- Design secure CV file storage with Amazon S3.
- Prepare an EC2 environment for running the FastAPI backend.
- Configure basic IAM and Security Group settings for the backend.

### Work Completed

| Day | Task | Start Date | Completion Date | Reference |
| --- | --- | --- | --- | --- |
| Day 1 | Study S3 private buckets and IAM Roles<br>Avoid exposing CV files publicly and let the backend control access | 2026-07-13 | 2026-07-13 | Amazon S3 Docs / IAM Docs |
| Day 2 | Design storage references and CV upload<br>Store only object keys in the database and validate files before upload | 2026-07-14 | 2026-07-14 | Amazon S3 Docs / Boto3 Docs |
| Day 3 | Prepare EC2 for the backend<br>Install Python, virtual environment, dependencies, and run Uvicorn | 2026-07-15 | 2026-07-15 | Amazon EC2 Docs / FastAPI Docs |
| Day 4 | Configure Security Groups and test APIs<br>Open required ports, check the health endpoint, and verify backend access | 2026-07-16 | 2026-07-16 | Amazon EC2 Docs / Security Group Docs |

### Results

The backend can handle CV uploads more securely and has a clear trial deployment process on EC2. The team better understood how S3, IAM Roles, EC2, and Security Groups work together when deploying a backend to the cloud.
