---
title: "Tuần 8 - Kiểm thử, CloudWatch và hoàn thiện"
date: 2026-07-27
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu

- Kiểm thử luồng nghiệp vụ chính sau khi tích hợp backend, frontend và AWS.
- Theo dõi backend bằng CloudWatch Logs.
- Hoàn thiện demo và báo cáo thực tập.

### Công việc đã thực hiện

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu |
| --- | --- | --- | --- | --- |
| 2 | Test luồng company -> admin -> student<br>Đảm bảo bài đăng được duyệt trước khi student apply | 27/07/2026 | 27/07/2026 | Pytest Docs / Project tests |
| 3 | Test upload CV, phân quyền và validation<br>Kiểm tra kích thước file, presigned URL và truy cập sai role | 28/07/2026 | 28/07/2026 | Pytest Docs / Project tests |
| 4 | Cấu hình CloudWatch Logs và kiểm tra health endpoint<br>Theo dõi stdout/stderr, lỗi runtime và trạng thái backend | 29/07/2026 | 29/07/2026 | CloudWatch Logs Docs / Project checklist |
| 5 | Demo final flow và hoàn thiện báo cáo<br>Tổng hợp proposal, project, workshop, worklog và self-evaluation | 30/07/2026 | 30/07/2026 | Project checklist / Report outline |

### Kết quả đạt được

Dự án hoàn thiện ở mức demo thực tế với luồng company, admin và student rõ ràng. Nhóm có báo cáo mô tả đầy đủ problem, solution, kiến trúc, quá trình làm việc, triển khai AWS và kết quả học được.
