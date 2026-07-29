---
title: "Tuần 9 - EC2 và deploy backend"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu

- Tìm hiểu cách đưa FastAPI backend lên Amazon EC2.
- Cấu hình network và security group cơ bản.

### Công việc đã thực hiện

| Nội dung | Kết quả |
| --- | --- |
| Tạo EC2 instance | Chuẩn bị môi trường Linux cho backend |
| Cài Python, venv, dependencies | Backend có thể chạy bằng Uvicorn |
| Mở port kiểm thử | Cho phép truy cập API qua port 8000 tạm thời |
| Kiểm tra health endpoint | `/health` trả trạng thái service |

### Kết quả đạt được

Backend có quy trình deploy rõ ràng trên EC2. Nhóm hiểu hơn về security group, inbound rule, SSH và cách chạy service backend trong môi trường cloud.
