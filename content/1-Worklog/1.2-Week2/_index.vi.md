---
title: "Tuần 2 - Phân tích yêu cầu backend"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu

- Xác định các API chính cho student, company và admin.
- Thiết kế mô hình dữ liệu ban đầu.
- Chọn framework backend và thư viện cần sử dụng.

### Công việc đã thực hiện

| Nội dung | Kết quả |
| --- | --- |
| Phân rã chức năng theo role | Student, company, admin |
| Thiết kế database ban đầu | Users, profiles, companies, internship posts, applications |
| Chọn công nghệ backend | FastAPI, SQLAlchemy, Pydantic, Alembic |
| Xác định endpoint chính | Auth, internships, student, company, admin |

### Kết quả đạt được

Backend được định hướng theo REST API, có phân quyền theo role và có khả năng chạy local bằng SQLite trước khi chuyển sang PostgreSQL trên AWS RDS.
