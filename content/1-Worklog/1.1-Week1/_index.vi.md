---
title: "Worklog Tuần 1"
date: 2025-09-06
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Mục tiêu tuần 1:

* Hòa nhập văn hóa FCJ, thiết lập kênh giao tiếp và nhóm dự án.
* Thiết lập **AWS Landing Zone** cơ bản: Tài khoản, Bảo mật (IAM), Ngân sách (Billing).
* **Deep Dive Networking:** Hiểu tường tận luồng đi của gói tin trong VPC.

## Các công việc cần triển khai trong tuần này

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
|-----|-----------|--------------|-----------------|----------------|
| 2 | - **Onboarding:** Tham gia Kick-off, nắm bắt lộ trình và thành lập đội nhóm dự án (Team Building). | 06/09/2025 | 06/09/2025 | |
| 3 | - **Setup Environment:** Tạo tài khoản AWS Root.<br>- **Security First:** Kích hoạt MFA cho Root User, tạo IAM Admin User thay vì dùng Root.<br>- **FinOps:** Tạo AWS Budgets cảnh báo khi chi phí vượt quá $5. | 09/09/2025 | 09/09/2025 |  [cloudjourney.awsstudygroup.com](https://cloudjourney.awsstudygroup.com/) |
| 4 | - **Architecture Study:** Phân tích sơ đồ "VPC 3-tier" trên Draw.io.<br>- **AWS Support:** Tìm hiểu các gói hỗ trợ (Basic, Developer, Business) và cách mở case khi gặp sự cố. | 10/09/2025 | 10/09/2025 |  [cloudjourney.awsstudygroup.com](https://cloudjourney.awsstudygroup.com/) |
| 5 | - **VPC Implementation:**<br>&emsp;+ Khởi tạo VPC với CIDR Block `10.0.0.0/16`.<br>&emsp;+ **Subnetting:** Chia dải mạng thành Public Subnet (cho Web Server) và Private Subnet (cho DB).<br>&emsp;+ **Routing:** Cấu hình Internet Gateway (IGW) và Route Table để Public Subnet ra được Internet.<br>&emsp;+ **Firewall:** Tạo Security Group mở port 22 (SSH) và 80 (HTTP). | 11/09/2025 | 14/09/2025 | Hoàn thành Lab VPC |

## Kết quả đạt được tuần 1

* Tham gia buổi kick-off và làm quen với các thành viên trong First Cloud Journey.
* Hiểu về tổ chức và các mục tiêu của chương trình.
* Thành công tạo nhóm để thực hiện các dự án.
* Tạo tài khoản AWS thành công và thực hiện các thao tác cơ bản:
  * Tạo IAM groups.
  * Kích hoạt bảo mật hai lớp (MFA).
* Đã thiết lập môi trường AWS an toàn, kiểm soát được rủi ro về chi phí (Cost Budget).
* Hiểu rõ bản chất của **VPC**: Là một trung tâm dữ liệu ảo hóa biệt lập.
* Phân biệt được sự khác nhau giữa **Public Subnet** (có Route ra IGW) và **Private Subnet** (không có Route trực tiếp ra Internet).
* Thành thạo việc quy hoạch địa chỉ IP (CIDR) để tránh xung đột mạng sau này.