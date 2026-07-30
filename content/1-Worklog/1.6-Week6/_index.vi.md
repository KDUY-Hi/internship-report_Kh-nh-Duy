---
title: "Tuần 6 - S3 và deploy backend trên EC2"
date: 2026-07-13
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu

- Thiết kế cách lưu file CV an toàn bằng Amazon S3.
- Chuẩn bị môi trường EC2 để chạy FastAPI backend.
- Cấu hình IAM và Security Group cơ bản cho backend.

### Công việc đã thực hiện

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Tìm hiểu S3 private bucket và IAM Role<br>Không public CV trực tiếp, backend kiểm soát quyền truy cập | 13/07/2026 | 13/07/2026 | Amazon S3 Docs / IAM Docs |
| 3 | Thiết kế storage reference và upload CV<br>Database chỉ lưu object key, backend kiểm tra file trước khi upload | 14/07/2026 | 14/07/2026 | Amazon S3 Docs / Boto3 Docs |
| 4 | Chuẩn bị EC2 cho backend<br>Cài Python, virtual environment, dependencies và chạy Uvicorn | 15/07/2026 | 15/07/2026 | Amazon EC2 Docs / FastAPI Docs |
| 5 | Cấu hình Security Group và kiểm tra API<br>Mở port cần thiết, kiểm tra health endpoint và quyền truy cập backend | 16/07/2026 | 16/07/2026 | Amazon EC2 Docs / Security Group Docs |

### Kết quả đạt được

Backend có thể xử lý upload CV theo hướng bảo mật hơn và có quy trình chạy thử trên EC2. Nhóm hiểu rõ hơn cách kết hợp S3, IAM Role, EC2 và Security Group khi triển khai backend lên môi trường cloud.
