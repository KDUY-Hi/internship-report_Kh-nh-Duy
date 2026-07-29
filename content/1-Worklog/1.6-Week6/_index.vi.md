---
title: "Tuần 6 - Upload CV và S3"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu

- Thiết kế cách lưu file CV an toàn.
- Tích hợp backend với Amazon S3.
- Đảm bảo chỉ người có quyền mới xem được CV.

### Công việc đã thực hiện

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Tìm hiểu S3 private bucket<br>Không public CV trực tiếp | 15/09/2025 | 15/09/2025 | Amazon S3 Docs / Boto3 Docs |
| 3 | Thiết kế storage reference<br>Database chỉ lưu object key | 16/09/2025 | 16/09/2025 | Amazon S3 Docs / Boto3 Docs |
| 4 | Upload CV qua backend<br>Backend kiểm tra file và lưu lên S3 | 17/09/2025 | 17/09/2025 | Amazon S3 Docs / Boto3 Docs |
| 5 | Presigned URL<br>Company xem CV qua URL tạm thời | 18/09/2025 | 18/09/2025 | Amazon S3 Docs / Boto3 Docs |

### Kết quả đạt được

CV được xử lý theo hướng bảo mật hơn: file nằm trong S3 private bucket, backend kiểm soát quyền truy cập và chỉ tạo presigned URL ngắn hạn cho user hợp lệ.
