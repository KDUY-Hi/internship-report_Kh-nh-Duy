---
title: "Week 11 - Frontend Deployment"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

# Week 11 - Frontend Deployment

### Goals

- Build the React app for production.
- Deploy the frontend to S3 Static Website Hosting or CloudFront.
- Configure CORS between the frontend and backend.

### Work Completed

| Task | Result |
| --- | --- |
| Configure `VITE_API_URL` | Frontend calls the production backend |
| Build frontend | Created the Vite `dist` folder |
| Upload to S3 | Served static assets through S3/CloudFront |
| Configure backend CORS | Allowed only the valid frontend domain |

### Results

The frontend can be accessed from a browser through AWS hosting. The application connects to the production backend and is ready for an end-to-end demo.
