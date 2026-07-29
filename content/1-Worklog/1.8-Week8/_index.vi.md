---
title: "Tuần 8 - Kiểm thử và sửa lỗi"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

# Tuần 8 - Kiểm thử và sửa lỗi

### Mục tiêu

- Kiểm thử luồng nghiệp vụ chính.
- Bổ sung validation và xử lý lỗi.

### Công việc đã thực hiện

| Nội dung | Kết quả |
| --- | --- |
| Test luồng company -> admin -> student | Đảm bảo bài đăng phải được duyệt trước khi student apply |
| Test upload CV | Kiểm tra kích thước file và quyền xem CV |
| Test phân quyền | Chặn truy cập sai role |
| Test notification | Tạo thông báo khi trạng thái thay đổi |

### Kết quả đạt được

Dự án ổn định hơn cho demo. Các trường hợp lỗi như ứng tuyển trùng, deadline hết hạn, tài khoản bị khóa và truy cập sai quyền được xử lý rõ ràng.
