---
title: "Worklog Tuần 6"
date: 2025-10-14
weight: 6
chapter: false
pre: "<b>1.6. </b>"
---

> **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn kể cả lưu ý này.

## Mục tiêu tuần 6

- Làm chủ hệ sinh thái lưu trữ **AWS Storage** (S3, Backup, Gateway).
- Tiếp cận tư duy **DevSecOps** và công cụ hỗ trợ code AI.
- Refactor cấu trúc dự án dựa trên kiến thức mới.

## Các công việc cần triển khai trong tuần này

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
|-----|----------|--------------|-----------------|----------------|
| 2 | - **Amazon S3:**<br>&emsp;+ Cấu hình Bucket Policy để host Static Website.<br>&emsp;+ Tìm hiểu S3 Storage Classes (Standard, IA, Glacier) và quy tắc chuyển đổi (Lifecycle Rule) để tối ưu chi phí. | 14/10/2025 | 15/10/2025 | [Tham khảo tại đây](https://aws.amazon.com/s3/) |
| 3 | - **Hybrid Storage:** Tìm hiểu AWS Storage Gateway để mở rộng ổ cứng on-prem lên cloud.<br>- **Webinar:** Tham gia "Reinventing DevSecOps with AWS Generative AI". | 16/10/2025 | 17/10/2025 | [Tham khảo tại đây](https://aws.amazon.com/storagegateway/) <br> [Webinar DevSecOps](https://aws.amazon.com/events/) |
| 4 | - **Data Resiliency:** Nghiên cứu chiến lược Backup & Restore (RTO/RPO).<br>- Cấu hình **AWS Backup** plan để tự động sao lưu dữ liệu. | 18/10/2025 | 19/10/2025 | [Tham khảo tại đây](https://aws.amazon.com/backup/) |
| 5 | - **GenAI for Dev:** Trải nghiệm **Amazon Q Developer** để hỗ trợ giải thích code và scan lỗ hổng bảo mật.<br>- Tinh chỉnh lại sơ đồ kiến trúc dự án sau khi hiểu thêm về các dịch vụ Storage. | 20/10/2025 | 21/10/2025 |    [Amazon Q Developer](https://aws.amazon.com/q/developer/) |

## Kết quả đạt được tuần 6

- Hiểu rõ sự khác biệt giữa Block Storage (EBS) và Object Storage (S3), biết khi nào dùng cái nào.
- Nắm được quy trình vòng đời dữ liệu (Data Lifecycle) để không trả tiền cho dữ liệu "lạnh" với giá "nóng".
- Tiếp thu tư duy **Shift-Left Security** từ Webinar: Đưa bảo mật vào sớm trong quy trình phát triển thay vì đợi đến cuối.
- Biết cách sử dụng Amazon Q để tăng tốc độ code và rà soát lỗi cơ bản.