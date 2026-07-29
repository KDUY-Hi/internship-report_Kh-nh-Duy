---
title: "Week 2 - Backend Requirement Analysis"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Goals

- Identify the main APIs for students, companies, and admins.
- Design the initial data model.
- Select the backend framework and required libraries.

### Work Completed

| Task | Result |
| --- | --- |
| Break down features by role | Student, company, and admin |
| Design the initial database | Users, profiles, companies, internship posts, applications |
| Select backend technologies | FastAPI, SQLAlchemy, Pydantic, Alembic |
| Define core endpoints | Auth, internships, student, company, admin |

### Results

The backend was designed as a REST API with role-based authorization and the ability to run locally with SQLite before moving to PostgreSQL on Amazon RDS.
