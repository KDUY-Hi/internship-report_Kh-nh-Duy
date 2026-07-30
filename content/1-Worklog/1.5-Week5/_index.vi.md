---
title: "Tuần 5 - Chuẩn bị S3, RDS và EC2"
date: 2026-07-06
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu

- Chuẩn bị các dịch vụ AWS cốt lõi cho project.
- Thiết kế cách lưu CV bằng S3 private bucket.
- Lên kế hoạch triển khai backend trên EC2 và database trên RDS PostgreSQL.

### Công việc đã thực hiện

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Tìm hiểu Amazon S3 cho file storage<br>Thiết kế bucket private để lưu CV và tránh public dữ liệu nhạy cảm | 06/07/2026 | 06/07/2026 | Amazon S3 Docs |
| 3 | Tìm hiểu Amazon RDS PostgreSQL<br>Xác định database production, subnet, security group và quy trình migration | 07/07/2026 | 07/07/2026 | Amazon RDS Docs / PostgreSQL Docs |
| 4 | Tìm hiểu Amazon EC2 cho backend<br>Chuẩn bị mô hình chạy FastAPI bằng Uvicorn trên Linux server | 08/07/2026 | 08/07/2026 | Amazon EC2 Docs / FastAPI Docs |
| 5 | Lập checklist triển khai AWS<br>Tổng hợp biến môi trường, secret, inbound rule, CORS và bước kiểm thử sau deploy | 09/07/2026 | 09/07/2026 | AWS Docs / Project checklist |

### Kết quả đạt được

Nhóm có kế hoạch triển khai AWS rõ ràng hơn trước khi bắt đầu cấu hình thực tế. Các thành phần S3, RDS và EC2 được xác định vai trò cụ thể trong kiến trúc project.
