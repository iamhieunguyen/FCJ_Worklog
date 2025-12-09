---
title: "Worklog Tuần 7"
date: 2025-10-21
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

> ⚠️ **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn kể cả warning này.

### Mục tiêu tuần 7: 

* Hệ thống hóa toàn bộ kiến thức AWS Core (Compute, Network, Storage, Security).
* Luyện tập phản xạ giải quyết vấn đề thông qua các bài Lab/Test.
* Chuẩn bị tâm thế tốt nhất cho kỳ thi giữa kỳ.

---

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| 2 | - **Compute Review:** So sánh EC2 vs Lambda. Khi nào nên dùng Serverless?<br>- **Lab:** Cấu hình User Data để bootstrap EC2 instance tự động cài web server. | 22/10/2025 | 22/10/2025 | AWS Builders, AWSboy |
| 3 | - **Storage Review:** Phân biệt các use-case của S3, EBS, EFS.<br>- **Lab:** Mount EFS vào nhiều EC2 instance để chia sẻ file. | 23/10/2025 | 23/10/2025 | AWS Builders, AWSboy |
| 4 | - **Network Consolidation:** Vẽ lại luồng packet từ Internet -> IGW -> Route Table -> NACL -> SG -> EC2.<br>- Làm bài test trên **AWSboy** để kiểm tra lỗ hổng kiến thức VPC. | 24/10/2025 | 24/10/2025 | AWS Builders, AWSboy |
| 5 | - **Security & DB:** Ôn tập IAM Roles (ủy quyền cho dịch vụ) vs IAM Users.<br>- So sánh RDS (SQL) và DynamoDB (NoSQL). | 25/10/2025 | 25/10/2025 | |
| 6 | - **Mock Exam:** Làm đề thi thử tổng hợp trên AWS Builders.<br>- Rà soát các câu sai, tìm đọc lại tài liệu trắng (Whitepaper) liên quan. | 26/10/2025 | 26/10/2025 | Exam Prep |

---

### Kết quả đạt được tuần 7: 

* Đã hoàn thành việc **ôn tập toàn diện** các nhóm dịch vụ AWS cơ bản: Compute, Storage, Networking, Database, Security (IAM).
* **Luyện tập thành công** hàng loạt bài lab và câu hỏi trắc nghiệm trên hai nền tảng miễn phí **AWS Builders** và **AWSboy**.
* Đã xâu chuỗi được các dịch vụ rời rạc thành một hệ thống liên kết: EC2 chạy trong VPC, dùng IAM Role để ghi dữ liệu vào S3.
* Tự tin với khả năng cấu hình mạng (Networking) và xử lý các vấn đề về phân quyền (Permission).
* Sẵn sàng kiến thức và kỹ năng cho kỳ thi đánh giá năng lực.