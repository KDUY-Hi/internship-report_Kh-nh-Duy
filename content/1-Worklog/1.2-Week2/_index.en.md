---
title: "Week 2 - Backend Requirement Analysis"
date: 2026-06-15
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
| Day 1 | Break down features by role<br>Student, company, and admin | 2026-06-15 | 2026-06-15 | FastAPI Docs / SQLAlchemy Docs |
| Day 2 | Design the initial database<br>Users, profiles, companies, internship posts, applications | 2026-06-16 | 2026-06-16 | FastAPI Docs / SQLAlchemy Docs |
| Day 3 | Select backend technologies<br>FastAPI, SQLAlchemy, Pydantic, Alembic | 2026-06-17 | 2026-06-17 | FastAPI Docs / SQLAlchemy Docs |
| Day 4 | Define core endpoints<br>Auth, internships, student, company, admin | 2026-06-18 | 2026-06-18 | FastAPI Docs / SQLAlchemy Docs |

### Results

The backend was designed as a REST API with role-based authorization and the ability to run locally with SQLite before moving to PostgreSQL on Amazon RDS.
