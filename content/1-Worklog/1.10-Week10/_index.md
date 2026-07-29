---
title: "Week 10 - RDS PostgreSQL"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

# Week 10 - RDS PostgreSQL

### Goals

- Move the production database to Amazon RDS PostgreSQL.
- Connect the EC2 backend to RDS securely.

### Work Completed

| Task | Result |
| --- | --- |
| Create RDS PostgreSQL | Production database `internship_portal` |
| Configure security group | Only EC2 backend can access port 5432 |
| Update `DATABASE_URL` | Backend connects to RDS instead of SQLite |
| Run Alembic migration | Create production schema |

### Results

The database is separated from the backend server, which better matches cloud architecture. Alembic keeps the local and production schemas consistent.
