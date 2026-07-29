---
title: "Tuần 11 - Deploy frontend"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu

- Build React app cho môi trường production.
- Deploy frontend lên S3 Static Website Hosting hoặc CloudFront.
- Cấu hình CORS giữa frontend và backend.

### Công việc đã thực hiện

| Nội dung | Kết quả |
| --- | --- |
| Cấu hình `VITE_API_URL` | Frontend gọi đúng backend production |
| Build frontend | Tạo thư mục `dist` bằng Vite |
| Upload lên S3 | Public static assets qua S3/CloudFront |
| Cấu hình CORS backend | Chỉ cho phép frontend domain hợp lệ |

### Kết quả đạt được

Frontend có thể truy cập từ trình duyệt thông qua AWS hosting. Ứng dụng kết nối được backend production và sẵn sàng cho luồng demo end-to-end.
