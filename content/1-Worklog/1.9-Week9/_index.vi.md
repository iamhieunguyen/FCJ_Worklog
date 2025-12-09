---
title: "Worklog Tuần 9"
date: 2025-11-04
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

> ⚠️ **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn.

### Mục tiêu tuần 9: 

* **Infrastructure as Code (IaC):** Chuyển đổi toàn bộ tài nguyên thủ công sang định nghĩa bằng code với **AWS SAM (Serverless Application Model)**.
* **Environment Consistency:** Loại bỏ hội chứng "It works on my machine" bằng cách container hóa môi trường build với **Docker**.
* **Deployment Strategy:** Thiết lập chiến lược triển khai tin cậy lên môi trường Cloud (Dev/Staging).

---

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| 2 | - **IaC Definition** | - Phân tích và viết file `template.yaml` để định nghĩa các tài nguyên serverless: Lambda Functions, API Gateway, DynamoDB Table.<br>- Áp dụng **SAM Policy Templates** để cấp quyền tối thiểu (Least Privilege) cho Lambda. | 04/11/2025 | 04/11/2025 | CloudFormation |
| 3 | - **Containerization** | - Tích hợp **Docker** vào quy trình `sam build`.<br>- Giải quyết vấn đề tương thích thư viện nhị phân (binary dependencies) của Python khi deploy từ Windows/Mac lên môi trường Linux của AWS Lambda. | 05/11/2025 | 06/11/2025 | Build Runtime |
| 4 | - **Troubleshooting** | - Gặp lỗi khi giả lập API Gateway cục bộ (`sam local start-api`) do thiếu kết nối mạng tới các AWS Service thực tế.<br>- Phân tích log build container để fix lỗi thiếu thư viện OS. | 06/11/2025 | 07/11/2025 | Debugging |
| 5 | - **Deployment Shift** | - Quyết định chuyển từ *Local Testing* sang chiến lược **Cloud-based Development**.<br>- Provisioning một môi trường `dev` riêng biệt trên AWS để kiểm thử tích hợp (Integration Test) chính xác nhất. | 07/11/2025 | 08/11/2025 | Shift-Right Testing |
| 6 | - **Milestone** | - Thực hiện lệnh `sam deploy --guided` thành công lần đầu tiên.<br>- Xác thực (Verify) các API Endpoints hoạt động ổn định trên hạ tầng thực tế. | 08/11/2025 | 08/11/2025 | Deployment |

---

### Kết quả đạt được tuần 9: 

* Đã "mã hóa" thành công toàn bộ hạ tầng dự án (IaC), cho phép tái tạo môi trường nhanh chóng chỉ với 1 lệnh deploy.
* Chuẩn hóa quy trình đóng gói ứng dụng (Packaging) thông qua Docker, đảm bảo tính nhất quán giữa Development và Production.
* Hệ thống backend đã sẵn sàng trên Cloud để đội Frontend bắt đầu tích hợp.