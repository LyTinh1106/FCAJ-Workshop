---
title: "Worklog Tuần 2"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

* Hiểu các khái niệm cốt lõi về kiến trúc và mạng của Amazon Virtual Private Cloud (VPC).
* Tìm hiểu cách các subnet public và private cô lập tài nguyên trong khi vẫn cho phép giao tiếp có kiểm soát.
* Cấu hình các thành phần mạng thiết yếu, bao gồm Internet Gateway, Route Tables và Security Groups.
* Triển khai các instance Amazon EC2 trong cả subnet public và private tuân theo các tiêu chuẩn mạng tốt nhất của AWS.
* Hiểu cách Elastic IP và NAT Gateway cung cấp kết nối Internet chiều đi (outbound) an toàn cho các tài nguyên trong mạng riêng (private).
* Xác thực kết nối giữa các tài nguyên AWS và phân tích luồng lưu lượng mạng trong môi trường VPC.
* Tích lũy kinh nghiệm thực hành trong việc thiết kế cơ sở hạ tầng mạng AWS an toàn và có khả năng mở rộng cho các ứng dụng đám mây trong tương lai.

### Các công việc cần triển khai trong tuần này:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Lab 03 - VPC Preparation**<br>- Tạo VPC<br>- Cấu hình khối CIDR<br>- Tạo subnet public và private | 27/04/2026 | 27/04/2026 | [Lab 03: Amazon VPC and AWS Site-to-Site VPN Workshop](https://000003.awsstudygroup.com/) |
| 3 | **Cấu hình các thành phần mạng**<br>- Tạo Internet Gateway<br>- Gắn Internet Gateway vào VPC<br>- Tạo Public & Private Route Tables<br>- Liên kết Route Tables với các subnet | 28/04/2026 | 28/04/2026 | [Lab 03: Amazon VPC and AWS Site-to-Site VPN Workshop](https://000003.awsstudygroup.com/) |
| 4 | **Triển khai các instance EC2**<br>- Tạo các Security Group<br>- Khởi chạy instance EC2 trong Public Subnet<br>- Khởi chạy instance EC2 trong Private Subnet | 29/04/2026 | 29/04/2026 | [Lab 03: Amazon VPC and AWS Site-to-Site VPN Workshop](https://000003.awsstudygroup.com/) |
| 5 | **Xác thực kết nối**<br>- Kết nối tới Public EC2 qua SSH<br>- Xác thực giao tiếp giữa Public và Private EC2<br>- Kiểm tra khả năng truy cập Internet từ mỗi subnet | 30/04/2026 | 30/04/2026 | [Lab 03: Amazon VPC and AWS Site-to-Site VPN Workshop](https://000003.awsstudygroup.com/) |
| 6 | **Cho phép truy cập Internet từ mạng riêng**<br>- Cấp phát Elastic IP<br>- Tạo NAT Gateway<br>- Cập nhật Private Route Table<br>- Xác thực kết nối Internet chiều đi (outbound) từ instance EC2 private | 01/05/2026 | 01/05/2026 | [Lab 03: Amazon VPC and AWS Site-to-Site VPN Workshop](https://000003.awsstudygroup.com/) |

### Kết quả đạt được tuần 2:

* **Thiết kế cấu trúc mạng VPC an toàn**: Xây dựng một Amazon VPC tùy chỉnh với các khối CIDR được hoạch định hợp lý, phân chia các khối lượng công việc vào các subnet public và private để nâng cao tính bảo mật và tổ chức mạng.
* **Cấu hình các thành phần mạng cốt lõi**: Tạo và tích hợp thành công Internet Gateway, Route Tables cùng các liên kết subnet để thiết lập luồng lưu lượng truy cập inbound và outbound có kiểm soát.
* **Triển khai các biện pháp kiểm soát bảo mật mạng**: Cấu hình các Security Group với các quy tắc inbound và outbound phù hợp, đảm bảo chỉ lưu lượng truy cập được ủy quyền mới có thể tiếp cận các instance EC2 trong khi vẫn duy trì sự cô lập mạng.
* **Triển khai tài nguyên máy chủ nhiều tầng (Multi-tier Compute)**: Khởi chạy các instance Amazon EC2 trong cả subnet public và private, xác thực các mô hình giao tiếp an toàn giữa các tài nguyên được triển khai ở các phân vùng mạng khác nhau.
* **Cho phép truy cập Internet chiều đi an toàn**: Cấp phát một Elastic IP, triển khai NAT Gateway và cập nhật các route table riêng để cho phép các instance EC2 private truy cập vào các kho lưu trữ phần mềm và dịch vụ bên ngoài mà không để chúng tiếp xúc trực tiếp với lưu lượng Internet chiều vào.
* **Xác thực kết nối đầu-cuối**: Thực hiện các bài kiểm tra kết nối để xác thực quyền truy cập SSH vào các instance public, giao tiếp giữa các instance public và private, cũng như kết nối Internet chiều đi qua NAT Gateway.
* **Củng cố kiến thức về mạng AWS**: Tích lũy kinh nghiệm thực tế trong thiết kế, cấu hình, xử lý sự cố và xác thực hạ tầng mạng AWS, tạo nền tảng vững chắc để triển khai các ứng dụng đám mây bảo mật và có độ khả dụng cao trong các bài thực hành tiếp theo.
