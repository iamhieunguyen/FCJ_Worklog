---
title: "Worklog Tuần 3"
date: 2025-09-21
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---


### Mục tiêu tuần 3:

* Giải quyết bài toán phân giải tên miền lai (**Hybrid DNS**) giữa On-premise và Cloud.
* Kết nối mạng giữa các VPC khác nhau bằng **VPC Peering**.
* Khắc phục sự cố tài khoản (nếu có).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
|---|---|---|---|---|
| 2 | - **Account Recovery:** Xử lý các vấn đề về thẻ thanh toán/tài khoản AWS để đảm bảo môi trường thực hành liên tục. | 21/09/2025 | 23/09/2025 | |
| 3 | - **Route 53 Resolver:**<br>&emsp;+ Cấu hình **Inbound Endpoint**: Cho phép On-prem resolve domain trên AWS.<br>&emsp;+ Cấu hình **Outbound Endpoint**: Cho phép AWS resolve domain dưới On-prem.<br>- Thực hành Lab DNS forwarding. | 24/09/2025 | 25/09/2025 | [Tham khảo tại đây](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 4 | - **VPC Peering Setup:**<br>&emsp;+ Khởi tạo 2 VPC riêng biệt.<br>&emsp;+ Tạo Peering Connection Request -> Accept.<br>&emsp;+ **Routing:** Cập nhật Route Table của cả 2 VPC để trỏ dải IP của nhau về Peering Connection (`pcx-xxx`). | 25/09/2025 | 26/09/2025 | [Tham khảo tại đây](https://youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&si=NtlkPHvTydrkH4rK) |
| 5 | - **Project Planning:** Họp nhóm, thảo luận về ý tưởng dự án cuối khóa dựa trên các dịch vụ đã học. | 28/09/2025 | 28/09/2025 | |


### Kết quả đạt được tuần 3:

* Tạo lại thành công tài khoản AWS mới để tiếp tục học tập, Tiếp tục được đồng hành cùng FCJ team.

* Hiểu rõ về Route 53 và cách thiết lập các quy tắc (Rules):
    * Tìm hiểu và tạo Outbound Endpoint.
    * Tìm hiểu và tạo Route 53 Resolver.
    * Tìm hiểu và tạo Inbound Endpoints.
    * Thực hành và kết nối thành công với RD Gateway Server.

* Nắm vững cơ chế hoạt động của **Route 53 Resolver**, giải quyết được bài toán giao tiếp DNS phức tạp trong môi trường Hybrid.
* Hiểu rõ giới hạn và cách cấu hình **VPC Peering**:
    * Peering không có tính chất bắc cầu (Transitive Peering).
    * Phải cấu hình Route Table ở cả hai đầu.
    * Cần bật tính năng "DNS Resolution" trong Peering Options để phân giải Private IP.
* Ổn định hạ tầng tài khoản để sẵn sàng cho các bài Lab nâng cao.