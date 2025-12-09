---
title: "Worklog Tuần 8"
date: 2025-10-28
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8: 

* **Milestone:** Hoàn thành kỳ thi giữa kỳ.
* **Architectural Pivot:** Chuyển đổi tư duy sang thiết kế hệ thống **Serverless** cho dự án *Travel Journal*.
* **Implementation:** Bắt đầu code các chức năng backend lõi (CRUD) và tích hợp AI.

---

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| 2 | - **Final Review:** Rà soát lại các kiến thức về Security Group Inbound/Outbound rules lần cuối trước giờ G. | 28/10/2025 | 28/10/2025 | Ghi chú cá nhân, AWS Builders |
| 3 | - **Project Setup:** Khởi tạo môi trường phát triển (IDE, AWS CLI profiles).<br>- Cấu hình **DynamoDB** với thiết kế Single Table (nếu cần) hoặc Multi-table cho bài viết/users. | 29/10/2025 | 30/10/2025 | |
| 4 | - **Exam Day:** Tham gia kỳ thi giữa kỳ.<br>- Họp team sau thi để re-plan lại tiến độ dự án. | 31/10/2025 | 31/10/2025 | |
| 5 | - **Serverless Backend:**<br>&emsp;+ Viết **Lambda Function** bằng Python (Boto3) cho chức năng `CreatePost` và `GetPost`.<br>&emsp;+ Tích hợp API Gateway để expose Lambda ra public endpoint. | 01/11/2025 | 01/11/2025 | FaaS Implementation |
| 6 | - **AI Integration Strategy:**<br>&emsp;+ Nghiên cứu SDK **AWS Rekognition**.<br>&emsp;+ Thiết kế luồng xử lý ảnh: Client upload S3 -> S3 Event Notification -> Lambda Trigger -> Rekognition (Detect Labels) -> Save Tags to DB. | 02/11/2025 | 02/11/2025 | Event-Driven Architecture |

---

### Kết quả đạt được tuần 8: 

* Đã vượt qua kỳ thi giữa kỳ, khẳng định nền tảng kiến thức vững chắc.
* Chính thức khởi động việc coding dự án **Travel Journal**.
* Đã thiết lập thành công luồng **API Serverless** đầu tiên: Client gọi API Gateway kích hoạt Lambda thao tác với DynamoDB.
* Có bản thiết kế chi tiết cho tính năng AI (xử lý ảnh tự động), chuyển từ mô hình xử lý đồng bộ sang bất đồng bộ (Event-driven) để tối ưu hiệu năng.