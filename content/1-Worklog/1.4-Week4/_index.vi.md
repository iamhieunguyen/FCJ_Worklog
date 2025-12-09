---
title: "Worklog Tuần 4"
date: 2025-09-29
weight: 4
chapter: false
pre: "<b>1.4. </b>"
---

> **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn kể cả lưu ý này.

## Mục tiêu tuần 4

* Chuyển đổi mô hình kết nối từ Peering sang **AWS Transit Gateway (TGW)**.
* Tìm hiểu sâu về các tính năng nâng cao của EC2 (Scaling, Pricing).
* Chuẩn hóa quy trình làm việc nhóm với **Git/GitHub**.
  
## Các công việc cần triển khai trong tuần này

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
|-----|----------|--------------|-----------------|----------------|
| 2 | - **Networking Advanced:** Triển khai **Transit Gateway**.<br>- So sánh TGW (Hub-and-Spoke) vs VPC Peering (Mesh). TGW giúp quản lý tập trung và đơn giản hóa routing khi số lượng VPC tăng lên. | 29/09/2025 | 30/09/2025 | [Tham khảo tại đây](https://aws.amazon.com/transit-gateway/) |
| 3 | - **EC2 Deep Dive:**<br>&emsp;+ **Auto Scaling Group (ASG):** Cơ chế tự động tăng/giảm server theo CPU/RAM.<br>&emsp;+ **Pricing Models:** Phân tích Spot Instances (tiết kiệm 90%) vs On-Demand vs Reserved. | 01/10/2025 | 02/10/2025 | [Tham khảo tại đây](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 4 | - **Source Control:**<br>&emsp;+ Thực hành các lệnh Git: `git clone`, `git branch`, `git checkout`, `git merge`.<br>&emsp;+ Xử lý xung đột (Merge Conflict) khi làm việc nhóm. | 03/10/2025 | 04/10/2025 | [Tham khảo tại đây](https://www.youtube.com/watch?v=8O14qT3jdq0&list=PLodO7Gi1F7R0t9SyEZF5mwfKevCULLjgG&index=2) |
| 5 | - **Pre-Proposal:** Brainstorm ý tưởng dự án, phân tích tính khả thi kỹ thuật và phân chia module (BE/FE/DevOps). | 05/10/2025 | 06/10/2025 | |

## Kết quả đạt được tuần 4

- Hiểu được **Transit Gateway** trong việc đơn giản hóa bảng định tuyến (Route Table) so với mớ hỗn độn của VPC Peering khi quy mô lớn.
- Nắm vững các đặc điểm chính của Amazon EC2:
  - Tính co giãn (Elasticity) để mở rộng hoặc thu hẹp tài nguyên theo nhu cầu.
  - Cấu hình linh hoạt cho các loại instance.
  - Tối ưu chi phí thông qua các mô hình định giá.
- Hiểu cách hoạt động của EC2 Auto Scaling để tự động điều chỉnh tài nguyên.
- Nắm được khái niệm về Instance Store trong dịch vụ lưu trữ của EC2.
- Nắm được chiến lược sử dụng EC2: Dùng Spot cho stateless app, Reserved cho database để tối ưu chi phí.
- Thành thạo quy trình **Git Flow** cơ bản, sẵn sàng cho việc code chung (collab) trong dự án sắp tới.