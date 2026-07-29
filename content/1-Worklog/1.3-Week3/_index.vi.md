---
title: "Tuần 3 - Authentication và database"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

# Tuần 3 - Authentication và database

### Mục tiêu

- Xây dựng đăng ký, đăng nhập và xác thực bằng JWT.
- Hoàn thiện các model cốt lõi.
- Thiết lập migration bằng Alembic.

### Công việc đã thực hiện

| Nội dung | Kết quả |
| --- | --- |
| Xây dựng bảng `users` | Lưu tài khoản, email, password hash, role |
| Cài đặt JWT authentication | Bảo vệ API bằng access token và refresh token |
| Tạo model hồ sơ | Student profile và company profile |
| Thiết lập Alembic | Quản lý thay đổi schema |

### Kết quả đạt được

Hệ thống có nền tảng đăng nhập và phân quyền ban đầu. Các API có thể xác định người dùng hiện tại và kiểm tra quyền trước khi xử lý nghiệp vụ.
