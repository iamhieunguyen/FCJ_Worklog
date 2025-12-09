---
title: "Worklog Tuần 2"
date: 2025-09-15
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---


## Mục tiêu tuần 2

* Làm chủ dịch vụ **Amazon EC2**: Từ khởi tạo đến kết nối SSH.
* Phân biệt và áp dụng **Security Group** vs **Network ACL (NACL)**.
* Cập nhật xu hướng công nghệ (AI/Data) qua sự kiện Cloud Day.

## Các công việc cần triển khai trong tuần này

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
|-----|-----------|--------------|-----------------|----------------|
| 2 | - **Theory:** Nghiên cứu các loại EC2 Instance (General Purpose, Compute Optimized...) và các dòng chip (Intel vs AWS Graviton).<br>- **Key Pair:** Tìm hiểu về mã hóa bất đối xứng (Public/Private key) để SSH an toàn. | 15/09/2025 | 16/09/2025 | |
| 3 | - **Provisioning:** Khởi tạo EC2 Instance (Ubuntu/Amazon Linux 2) trong Public Subnet.<br>- **Security Layering:**<br>&emsp;+ Cấu hình **Security Group** (Stateful Firewall) cấp Instance.<br>&emsp;+ Cấu hình **NACL** (Stateless Firewall) cấp Subnet để chặn IP độc hại. | 16/09/2025 | 17/09/2025 | [Tham khảo tại đây](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 4 | - **Troubleshooting:** Xử lý sự cố "Connection Time Out" khi SSH (thường do lỗi SG hoặc Route Table).<br>- Gửi yêu cầu xác thực tài khoản để tăng hạn ngạch (Quota). | 17/09/2025 | 20/09/2025 | [Tham khảo tại đây](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 5 | - **Event:** Tham gia **AWS Cloud Day**.<br>- **Insight:** Lắng nghe chia sẻ về Generative AI (Bedrock) và Data Analytics trong doanh nghiệp. | 18/09/2025 | 18/09/2025 | |

## Kết quả đạt được tuần 2

- Nắm được kiến thức cơ bản - nâng cao về VPC và EC2.
- Đã khởi chạy thành công máy chủ ảo đầu tiên trên Cloud và kết nối SSH an toàn.
- Hiểu sâu sắc cơ chế bảo mật nhiều lớp: NACL là "người gác cổng" khu phố (Subnet), Security Group là "bảo vệ" tòa nhà (Instance).
- Mở rộng tầm nhìn về ứng dụng thực tế của AI thông qua sự kiện Cloud Day, định hình hướng đi tương lai.