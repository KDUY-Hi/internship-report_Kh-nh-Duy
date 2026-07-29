---
title: "Week 6 - CV Upload and S3"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Goals

- Design a secure way to store CV files.
- Integrate the backend with Amazon S3.
- Ensure that only authorized users can view CVs.

### Work Completed

| Day | Task | Start Date | Completion Date | Reference |
| --- | --- | --- | --- | --- |
| Day 1 | Study S3 private buckets<br>CV files are not publicly exposed | 2025-09-15 | 2025-09-15 | Amazon S3 Docs / Boto3 Docs |
| Day 2 | Design storage references<br>Database stores only object keys | 2025-09-16 | 2025-09-16 | Amazon S3 Docs / Boto3 Docs |
| Day 3 | Upload CV through backend<br>Backend validates and stores files in S3 | 2025-09-17 | 2025-09-17 | Amazon S3 Docs / Boto3 Docs |
| Day 4 | Generate presigned URLs<br>Companies view CVs through temporary URLs | 2025-09-18 | 2025-09-18 | Amazon S3 Docs / Boto3 Docs |

### Results

CV files are handled more securely: files are stored in a private S3 bucket, backend controls access, and only authorized users receive short-lived presigned URLs.
