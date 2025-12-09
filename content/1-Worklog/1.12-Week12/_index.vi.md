---
title: "Worklog Tuần 12"
date: 2025-11-25
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---


### Mục tiêu tuần 12: 

* **Event-Driven Architecture (EDA):** Tích hợp **Amazon SQS** để xử lý bất đồng bộ (Asynchronous) cho tác vụ nặng (AI Processing).
* **Resilience & Reliability:** Đảm bảo hệ thống không bị mất dữ liệu khi lưu lượng truy cập tăng đột biến.
* **Production Readiness:** Cấu hình tên miền (Domain), chứng chỉ SSL và thông báo hệ thống (SNS).
* **Hoàn thiện các giao diện chính** của Frontend và **tham gia sự kiện AWS Cloud Mastery Series cuối cùng**.

---

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| 2 | - **Feature Completion** | - Hoàn thiện logic nghiệp vụ phức tạp cho chức năng `UpdateArticle` (xử lý concurrency khi nhiều user cùng sửa).<br>- Tinh chỉnh độ chính xác của AI Rekognition thông qua tham số `MinConfidence`. | 25/11/2025 | 25/11/2025 | Web Logic |
| 3 | - **Async Processing** | - **Architecture Upgrade:** Chuyển đổi luồng xử lý ảnh từ đồng bộ sang bất đồng bộ:<br> *Upload S3 -> S3 Event -> **SQS Queue** -> Lambda Worker -> DynamoDB*.<br>- Lợi ích: Decoupling (giảm sự phụ thuộc) và khả năng chịu tải cao (Throttling management). | 26/11/2025 | 26/11/2025 | SQS Integration |
| 4 | - **Geo-Location** | - Tích hợp tính năng **Map Pinning** trên Frontend.<br>- Lưu trữ tọa độ (Latitude/Longitude) vào DynamoDB và tối ưu hóa query địa lý (nếu cần). | 27/11/2025 | 27/11/2025 | Feature Dev |
| 5 | - **Notifications & Ops** | - Triển khai **Amazon SNS** để gửi email thông báo cho Admin khi có bài viết mới hoặc lỗi hệ thống (Alarm).<br>- Rà soát lại IAM Roles, đảm bảo nguyên tắc "Least Privilege" trước khi demo. | 28/11/2025 | 28/11/2025 | Operations |
| 6 | - **Go-Live Prep** | - Cấu hình **Route 53** để trỏ Custom Domain về CloudFront/S3.<br>- Request chứng chỉ SSL/TLS từ AWS Certificate Manager (ACM) để kích hoạt HTTPS.<br>- Tham gia buổi review cuối cùng để chốt phương án demo. | 29/11/2025 | 29/11/2025 | Final Polish |

---

### Kết quả đạt được tuần 12: 

* **Hệ thống đạt độ bền vững cao (Resiliency):** Nhờ việc đưa SQS vào làm bộ đệm (Buffer), hệ thống không bị "sập" ngay cả khi hàng nghìn ảnh được upload cùng lúc.
* **Kiến trúc hoàn chỉnh:** Một hệ thống Serverless tiêu chuẩn Enterprise với đầy đủ các thành phần: Compute (Lambda), Storage (S3), Database (DynamoDB), Integration (SQS/SNS), Network (API Gateway/Route53).
* **Tham gia thành công sự kiện AWS Cloud Mastery Series cuối cùng**, nhận được hướng dẫn tổng thể để hoàn thiện dự án.
* **Sẵn sàng Demo:** Sản phẩm hoạt động trơn tru trên môi trường Production với tên miền thực tế và bảo mật HTTPS.

