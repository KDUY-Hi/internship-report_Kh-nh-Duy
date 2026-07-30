---
title: "Tuần 7 - Frontend React và RDS PostgreSQL"
date: 2026-07-20
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu

- Hoàn thiện giao diện React cho các nhóm người dùng.
- Kết nối frontend với backend API.
- Chuẩn bị database production bằng Amazon RDS PostgreSQL.

### Công việc đã thực hiện

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Thiết lập React + Vite và API client<br>Quản lý request, token và lỗi phiên đăng nhập | 20/07/2026 | 20/07/2026 | React + Vite Docs / Project README |
| 3 | Xây dựng trang student, company và admin<br>Jobs, applications, profile, bài đăng, ứng viên, users và skills | 21/07/2026 | 21/07/2026 | React + Vite Docs / Project README |
| 4 | Tạo RDS PostgreSQL và cấu hình database production<br>Cập nhật `DATABASE_URL`, Security Group và Alembic migration | 22/07/2026 | 22/07/2026 | Amazon RDS Docs / Alembic Docs |
| 5 | Build frontend và cấu hình production<br>Thiết lập `VITE_API_URL`, kiểm tra CORS giữa frontend và backend | 23/07/2026 | 23/07/2026 | Vite Docs / CORS Docs |

### Kết quả đạt được

Frontend có thể thao tác với dữ liệu thật từ backend và database production được tách sang RDS PostgreSQL. Ứng dụng có cấu hình rõ ràng hơn giữa môi trường local và production.
