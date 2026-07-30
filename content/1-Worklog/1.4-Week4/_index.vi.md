---
title: "Tuần 4 - Kiến trúc AWS, IAM và Security Group"
date: 2026-06-29
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu

- Tìm hiểu kiến trúc triển khai project trên AWS.
- Nắm vai trò của IAM, VPC, subnet và Security Group.
- Xác định cách tách các thành phần frontend, backend, database và storage trong môi trường cloud.

### Công việc đã thực hiện

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Phân tích kiến trúc cloud tổng quan<br>Xác định frontend, backend, database và file storage sẽ chạy trên dịch vụ AWS nào | 29/06/2026 | 29/06/2026 | AWS Architecture Center / AWS Docs |
| 3 | Tìm hiểu IAM và nguyên tắc least privilege<br>Phân biệt IAM User, IAM Role, policy và quyền truy cập dịch vụ | 30/06/2026 | 30/06/2026 | IAM Docs / AWS Security Best Practices |
| 4 | Tìm hiểu VPC, subnet và routing cơ bản<br>Xác định vai trò public subnet, private subnet và cách đặt database an toàn hơn | 01/07/2026 | 01/07/2026 | Amazon VPC Docs |
| 5 | Thiết kế Security Group cho project<br>Giới hạn SSH, mở HTTP/HTTPS/API cần thiết và chỉ cho backend truy cập database | 02/07/2026 | 02/07/2026 | Security Group Docs / AWS Well-Architected |

### Kết quả đạt được

Nhóm xác định được kiến trúc AWS ban đầu cho project và hiểu rõ hơn cách kiểm soát quyền truy cập giữa các thành phần. Đây là bước chuẩn bị quan trọng trước khi tạo tài nguyên thật như S3, EC2 và RDS ở các tuần tiếp theo.
