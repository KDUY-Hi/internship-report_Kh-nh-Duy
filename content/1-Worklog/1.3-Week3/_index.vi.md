---
title: "Tuần 3 - Authentication và database"
date: 2026-06-22
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu

- Xây dựng đăng ký, đăng nhập và xác thực bằng JWT.
- Hoàn thiện các model cốt lõi.
- Thiết lập migration bằng Alembic.

### Công việc đã thực hiện

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Xây dựng bảng `users`<br>Lưu tài khoản, email, password hash, role | 22/06/2026 | 22/06/2026 | FastAPI Security / Alembic Docs |
| 3 | Cài đặt JWT authentication<br>Bảo vệ API bằng access token và refresh token | 23/06/2026 | 23/06/2026 | FastAPI Security / Alembic Docs |
| 4 | Tạo model hồ sơ<br>Student profile và company profile | 24/06/2026 | 24/06/2026 | FastAPI Security / Alembic Docs |
| 5 | Thiết lập Alembic<br>Quản lý thay đổi schema | 25/06/2026 | 25/06/2026 | FastAPI Security / Alembic Docs |

### Kết quả đạt được

Hệ thống có nền tảng đăng nhập và phân quyền ban đầu. Các API có thể xác định người dùng hiện tại và kiểm tra quyền trước khi xử lý nghiệp vụ.
