---
title: "Worklog Tuần 11"
date: 2025-11-18
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---


### Mục tiêu tuần 11: 

* **Tham gia sự kiện AWS Cloud Mastery Series #2** để tiếp tục giải đáp các vấn đề kỹ thuật chuyên sâu.
* **Architectural Refactoring:** Chuyển đổi từ Monolithic Stack sang kiến trúc **Multi-Stack** để giảm rủi ro deployment (Blast Radius).
* **Dependency Management:** Tối ưu hóa Lambda Layer để giảm kích thước gói deploy.
* **Pipeline Optimization:** Cải thiện tốc độ build và deploy.
---

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| CN | - **Knowledge Transfer** | - Cập nhật các pattern thiết kế Serverless nâng cao từ AWS Cloud Mastery Series #2 (Strangler Fig pattern, Fan-out). | 17/11/2025 | 17/11/2025 | Mentor, AWS Cloud Mastery Series |
| 2 | - **Stack Strategy** | - Phân tích file `template.yaml` (đang quá lớn) và quyết định tách thành các Nested Stacks:<br> 1. **Core-Infra Stack:** VPC, Security Groups (Ít thay đổi).<br> 2. **Data-Stack:** DynamoDB, S3 Buckets (Stateful).<br> 3. **App-Stack:** Lambda, API Gateway (Stateless - Deploy thường xuyên).| 18/11/2025 | 18/11/2025 | IaC Modularization |
| 3 | - **Implementation** | - Sử dụng `AWS::CloudFormation::Stack` resource để liên kết các stack con.<br>- Cấu hình `Outputs` và `Fn::ImportValue` để truyền tham số (VPC ID, Table Name) giữa các stack. | 19/11/2025 | 19/11/2025 | Cross-Stack Ref |
| 4 | - **Deployment Pipeline** | - Gặp lỗi "Circular Dependency" và "Export Name Collision" khi tách stack.<br>- **Fix:** Quy hoạch lại naming convention cho Export Values và thứ tự deploy.| 20/11/2025 | 20/11/2025 | CI/CD Troubleshooting |
| 5 | - **Code Optimization** | - Đóng gói các thư viện chung (`boto3`, `requests`, `utils`) vào **Lambda Layers**.<br>- Kết quả: Giảm dung lượng source code của từng function từ 10MB xuống <500KB, tăng tốc độ cold-start. | 21/11/2025 | 21/11/2025 | Performance |
| 6 | - **Stability** | - Finalize cấu trúc Multi-stack dự phòng.<br>- Đồng bộ hóa cấu trúc Frontend để tương thích với API Gateway mới tái cấu trúc.| 22/11/2025 | 22/11/2025 | System Stability |

---

### Kết quả đạt được tuần 11: 

* **Tham gia chuỗi sự kiện AWS Cloud Mastery Series #2**, thu thập thêm kiến thức sâu hơn về Serverless, Rekognition, và giải pháp cho các lỗi xác thực.
* Chuyển đổi thành công sang mô hình **Multi-Stack**: Giúp cô lập lỗi (Fault Isolation) và tăng tốc độ deploy (chỉ deploy lại stack có thay đổi).
* Hệ thống trở nên linh hoạt (Agile), dễ bảo trì và mở rộng hơn.
* Khắc phục triệt để các vấn đề phụ thuộc vòng (Circular Dependency) trong CloudFormation.
