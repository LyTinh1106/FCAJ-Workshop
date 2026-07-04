---
title: "Worklog Tuần 3"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:

* Hiểu kiến trúc DNS lai (hybrid DNS) sử dụng Amazon Route 53 Resolver.
* Tìm hiểu cách Route 53 Inbound và Outbound Resolver Endpoints cho phép giao tiếp DNS giữa AWS và môi trường on-premises.
* Triển khai và cấu hình hạ tầng Microsoft Active Directory (AD) cho các kịch bản mạng lai.
* Tích lũy kinh nghiệm thực hành với AWS CloudFormation để tự động hóa việc triển khai cơ sở hạ tầng.
* Hiểu kiến trúc và các trường hợp sử dụng của VPC Peering để giao tiếp riêng tư giữa các VPC bị cô lập.
* Cấu hình định tuyến, Network ACL, Security Group và phân giải DNS chéo (Cross-Peer DNS resolution) để cho phép kết nối liên VPC an toàn.
* Xác thực phân giải DNS và giao tiếp mạng trên các môi trường mạng lai và mạng kết nối chéo (peered networks).

### Các công việc cần triển khai trong tuần này:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Lab 10 - Set up Hybrid DNS with Route 53 Resolver**<br>- Chuẩn bị môi trường <br>- Tạo key pair<br>- Khởi tạo CloudFormation template<br>- Cấu hình các Security Group | 04/05/2026 | 04/05/2026 | [Lab 10: Set up Hybrid DNS with Route 53 Resolver](https://000010.awsstudygroup.com/) |
| 3 | **Triển khai hạ tầng Hybrid DNS**<br>- Kết nối tới Remote Desktop Gateway (RDGW)<br>- Triển khai Microsoft Active Directory<br>- Xác thực môi trường Active Directory | 05/05/2026 | 05/05/2026 | [Lab 10: Set up Hybrid DNS with Route 53 Resolver](https://000010.awsstudygroup.com/) |
| 4 | **Cấu hình Route 53 Resolver**<br>- Tạo Route 53 Outbound Endpoint<br>- Tạo các Route 53 Resolver Rule<br>- Tạo Route 53 Inbound Endpoint<br>- Xác thực phân giải DNS | 06/05/2026 | 06/05/2026 | [Lab 10: Set up Hybrid DNS with Route 53 Resolver](https://000010.awsstudygroup.com/) |
| 5 | **Lab 19 - VPC Peering Preparation**<br>- Triển khai các CloudFormation stack (my-vpc & hg-vpc)<br>- Tạo các Security Group<br>- Khởi chạy các instance EC2 trong cả hai VPC | 07/05/2026 | 07/05/2026 | [Lab 19: VPC Peering](https://000019.awsstudygroup.com/) |
| 6 | **Cấu hình VPC Peering**<br>- Tạo kết nối VPC Peering<br>- Cập nhật Route Tables<br>- Chỉnh sửa Network ACLs | 08/05/2026 | 08/05/2026 | [Lab 19: VPC Peering](https://000019.awsstudygroup.com/) |
| 7 | **Xác thực kết nối giữa các VPC**<br>- Kích hoạt Cross-Peer DNS Resolution<br>- Kiểm tra kết nối giữa các instance EC2 chéo VPC<br>- Xác thực phân giải tên miền DNS riêng tư | 09/05/2026 | 09/05/2026 | [Lab 19: VPC Peering](https://000019.awsstudygroup.com/) |

### Kết quả đạt được tuần 3:

* **Xây dựng hạ tầng Hybrid DNS**: Cấu hình Amazon Route 53 Resolver với Inbound và Outbound Endpoint, cho phép phân giải DNS liền mạch giữa tài nguyên AWS và môi trường Microsoft Active Directory on-premises.
* **Tự động hóa triển khai hạ tầng**: Tận dụng các mẫu AWS CloudFormation để cung cấp tài nguyên mạng và hạ tầng hỗ trợ, giảm cấu hình thủ công và cải thiện tính nhất quán trong triển khai.
* **Tích hợp Microsoft Active Directory với AWS**: Triển khai và cấu hình thành công Microsoft Active Directory cùng với Remote Desktop Gateway (RDGW), thiết lập nền tảng cho dịch vụ định danh và DNS lai.
* **Triển khai phân giải tên miền an toàn cho môi trường Hybrid**: Tạo các Route 53 Resolver Rule để chuyển tiếp truy vấn DNS giữa AWS và mạng on-premises, xác thực phân giải tên miền hai chiều thành công.
* **Thiết lập kết nối riêng tư giữa các VPC**: Cấu hình VPC Peering giữa hai VPC độc lập, cho phép giao tiếp riêng tư trực tiếp mà không cần đi qua Internet công cộng.
* **Cấu hình định tuyến và bảo mật mạng**: Cập nhật Route Tables, Network ACL và Security Group để định tuyến lưu lượng truy cập an toàn qua các VPC được kết nối trong khi vẫn duy trì sự cô lập mạng thích hợp.
* **Kích hoạt Cross-Peer DNS Resolution**: Cấu hình phân giải DNS trên các VPC được kết nối chéo, cho phép các instance EC2 giao tiếp bằng tên máy chủ DNS riêng tư thay vì địa chỉ IP.
* **Củng cố chuyên môn mạng AWS**: Tích lũy kinh nghiệm thực tế trong thiết kế các giải pháp mạng lai, tự động hóa triển khai hạ tầng và triển khai kết nối riêng tư an toàn giữa các môi trường AWS.
