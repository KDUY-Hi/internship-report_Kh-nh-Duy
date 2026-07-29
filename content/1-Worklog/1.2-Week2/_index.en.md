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

| Day | Task | Start Date | Completion Date | Reference |
| --- | --- | --- | --- | --- |
| Day 1 | Break down features by role<br>Student, company, and admin | 2025-08-18 | 2025-08-18 | FastAPI Docs / SQLAlchemy Docs |
| Day 2 | Design the initial database<br>Users, profiles, companies, internship posts, applications | 2025-08-19 | 2025-08-19 | FastAPI Docs / SQLAlchemy Docs |
| Day 3 | Select backend technologies<br>FastAPI, SQLAlchemy, Pydantic, Alembic | 2025-08-20 | 2025-08-20 | FastAPI Docs / SQLAlchemy Docs |
| Day 4 | Define core endpoints<br>Auth, internships, student, company, admin | 2025-08-21 | 2025-08-21 | FastAPI Docs / SQLAlchemy Docs |

### Results

The backend was designed as a REST API with role-based authorization and the ability to run locally with SQLite before moving to PostgreSQL on Amazon RDS.
