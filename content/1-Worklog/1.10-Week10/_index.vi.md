---
title: "Tuần 10 - RDS PostgreSQL"
date: 2024-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu

- Chuyển database production sang Amazon RDS PostgreSQL.
- Kết nối backend EC2 với RDS an toàn.

### Công việc đã thực hiện

| Nội dung | Kết quả |
| --- | --- |
| Tạo RDS PostgreSQL | Database `internship_portal` cho production |
| Cấu hình security group | Chỉ cho EC2 backend truy cập port 5432 |
| Cập nhật `DATABASE_URL` | Backend kết nối RDS thay vì SQLite |
| Chạy Alembic migration | Tạo schema production |

### Kết quả đạt được

Database được tách khỏi server backend, phù hợp hơn với kiến trúc cloud. Việc dùng Alembic giúp schema giữa local và production nhất quán.
