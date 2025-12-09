---
title: "Worklog Tuần 5"
date: 2025-10-07
weight: 5
chapter: false
pre: "<b>1.5. </b>"
---

> **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn kể cả lưu ý này.

## Mục tiêu tuần 5

* Thực hành **FinOps**: Điều tra và xử lý chi phí AWS bất thường.
* **System Design:** Phác thảo kiến trúc (Architecture Diagram) cho dự án.
* Khởi tạo dự án (Project Bootstrapping).

## Các công việc cần triển khai trong tuần này

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
|-----|----------|--------------|-----------------|----------------|
| 2 | - **Cost Analysis:** Sử dụng **AWS Cost Explorer** để truy vết nguồn gốc chi phí (phát hiện các EBS Volume mồ côi, Elastic IP không gắn vào instance).<br>- Thực hiện dọn dẹp tài nguyên (Cleanup). | 07/10/2025 | 08/10/2025 | [Tham khảo tại đây](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/) |
| 3 | - **Architecting:** Vẽ sơ đồ kiến trúc trên Draw.io.<br>- Quyết định mô hình: Frontend (S3/Amplify) + Backend (EC2/Lambda) + DB (RDS/DynamoDB). | 09/10/2025 | 10/10/2025 | [Tham khảo tại đây](https://www.facebook.com/groups/awsstudygroupfcj) |
| 4 | - **Code Skeleton:** Tạo cấu trúc thư mục chuẩn cho dự án.<br>- Thiết lập các file cấu hình môi trường (.env), `.gitignore` để tránh lộ Credential. | 11/10/2025 | 13/10/2025 | |
| 5 | - **Skill Builder:** Đăng ký các khóa học digital badge trên AWS Skill Builder để bổ sung kiến thức còn thiếu. | 11/10/2025 | 12/10/2025 | [Tham khảo tại đây](https://skillbuilder.aws/) |

## Kết quả đạt được tuần 5

- Hoàn thiện thiết kế kiến trúc hạ tầng dự án và đề xuất các mẫu tham khảo phù hợp cho nhóm.
- Hoàn thiện bản vẽ kiến trúc (Architecture Diagram) phiên bản 1.0, làm kim chỉ nam cho việc phát triển.
- Có được bộ khung dự án (Skeleton) sạch sẽ, tổ chức khoa học, sẵn sàng để team bắt tay vào code.
- Đã xác định và xử lý được nguyên nhân gây "rò rỉ" chi phí, học được bài học quan trọng về việc quản lý vòng đời tài nguyên.