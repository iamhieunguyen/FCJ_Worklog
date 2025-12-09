---
title: "Worklog Tuần 10"
date: 2025-11-11
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Mục tiêu tuần 10: 

* **Security Hardening:** Triển khai cơ chế xác thực tập trung (Authentication) và xử lý bảo mật trình duyệt (CORS).
* **System Integration:** Kết nối (Wiring) Frontend và Backend, đảm bảo luồng dữ liệu thông suốt.
* **Observability:** Theo dõi và gỡ lỗi hệ thống khi có tải thực tế.
* **Tham gia chuỗi sự kiện AWS Cloud Mastery Series** để nhận hướng dẫn và giải đáp thắc mắc về dự án.

---

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| 2 | - **Network Security** | - Cấu hình **CORS (Cross-Origin Resource Sharing)** chặt chẽ trên API Gateway.<br>- Refactor code Lambda để trả về đúng Headers bảo mật (`Access-Control-Allow-Origin`), ngăn chặn chặn request trái phép từ trình duyệt. | 11/11/2025 | 11/11/2025 | API Gateway Config |
| 3 | - **Data Flow** | - Tối ưu hóa truy vấn **DynamoDB**: Sử dụng GSI (Global Secondary Index) để tăng tốc độ đọc dữ liệu cho chức năng `GetArticles`.<br>- Chuẩn hóa định dạng JSON Response trả về cho Client.  | 12/11/2025 | 12/11/2025 | |
| 4 | - **Frontend Integration** | - Phối hợp deploy mã nguồn Frontend (React/Vue) lên S3 Static Hosting.<br>- Cấu hình biến môi trường (Environment Variables) để Frontend trỏ đúng tới API Endpoint của môi trường Dev. | 13/11/2025 | 13/11/2025 | CI/CD Prep |
| 5 | - **Identity Management** | - Tích hợp **Amazon Cognito User Pool**.<br>- Gặp lỗi `Sub ID` mismatch: Debug luồng xác thực JWT Token để đảm bảo Lambda nhận diện đúng User ID khi thực hiện thao tác xóa/sửa. | 14/11/2025 | 14/11/2025 |  Auth/Authz |
| 6 | - **Mentorship** | - Tham gia **AWS Cloud Mastery Series**: Review kiến trúc với chuyên gia.<br>- Nhận feedback về việc tách luồng xử lý ảnh (Image Processing) ra khỏi luồng upload chính để tránh timeout. | 15/11/2025 | 15/11/2025 | Architecture Review |

---

### Kết quả đạt được tuần 10: 

* Giải quyết triệt để vấn đề CORS - "cơn ác mộng" của mọi lập trình viên Frontend-Backend.
* Hệ thống đã có lớp bảo mật định danh (Identity Layer) với Cognito, đảm bảo chỉ user đã đăng nhập mới gọi được API.
* Hoàn thiện luồng chức năng Read/Delete trên giao diện người dùng thực tế.
* **Xác định và có hướng giải quyết** cho các điểm nghẽn quan trọng
* Dự án đã chuyển sang giai đoạn kiểm thử người dùng cơ bản.
