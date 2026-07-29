---
title: "Week 6 - CV Upload and S3"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

# Week 6 - CV Upload and S3

### Goals

- Design a secure way to store CV files.
- Integrate the backend with Amazon S3.
- Ensure that only authorized users can view CVs.

### Work Completed

| Task | Result |
| --- | --- |
| Study S3 private buckets | CV files are not publicly exposed |
| Design storage references | Database stores only object keys |
| Upload CV through backend | Backend validates and stores files in S3 |
| Generate presigned URLs | Companies view CVs through temporary URLs |

### Results

CV files are handled more securely: files are stored in a private S3 bucket, backend controls access, and only authorized users receive short-lived presigned URLs.
