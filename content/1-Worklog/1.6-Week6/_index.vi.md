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

| Nội dung | Kết quả |
| --- | --- |
| Tìm hiểu S3 private bucket | Không public CV trực tiếp |
| Thiết kế storage reference | Database chỉ lưu object key |
| Upload CV qua backend | Backend kiểm tra file và lưu lên S3 |
| Presigned URL | Company xem CV qua URL tạm thời |

### Kết quả đạt được

CV được xử lý theo hướng bảo mật hơn: file nằm trong S3 private bucket, backend kiểm soát quyền truy cập và chỉ tạo presigned URL ngắn hạn cho user hợp lệ.
