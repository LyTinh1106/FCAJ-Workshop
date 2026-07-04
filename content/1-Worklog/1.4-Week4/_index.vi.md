---
title: "Worklog Tuần 4"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* Hiểu kiến trúc và các trường hợp sử dụng của AWS Transit Gateway để kết nối nhiều Virtual Private Cloud (VPC).
* Tìm hiểu cách Transit Gateway đơn giản hóa mô hình mạng so với VPC Peering trong các môi trường AWS quy mô lớn.
* Cấu hình các kết nối (attachment) Transit Gateway và các bảng tuyến (route table) để cho phép giao tiếp có kiểm soát giữa nhiều VPC.
* Xác thực kết nối đầu-cuối qua các VPC liên kết với nhau bằng cách định tuyến tập trung.
* Hiểu các khái niệm cốt lõi của AWS Backup, bao gồm Backup Plans, Backup Vaults, policy vòng đời (lifecycle policies) và các điểm khôi phục (recovery points).
* Cấu hình lịch trình sao lưu tự động và cơ chế thông báo để nâng cao khả năng bảo vệ dữ liệu.
* Thực hiện khôi phục bản sao lưu và xác thực tính toàn vẹn của dữ liệu như một phần của việc thử nghiệm khôi phục sau sự cố (disaster recovery).
* Tích lũy kinh nghiệm thực tế trong thiết kế các chiến lược mạng có tính đàn hồi cao và chiến lược sao lưu theo các phương pháp tốt nhất của AWS.

### Các công việc cần triển khai trong tuần này:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Lab 20 - Transit Gateway**<br>- Tạo key pair (`tgw-key`)<br>- Khởi tạo CloudFormation template<br>- Triển khai hạ tầng mạng | 11/05/2026 | 11/05/2026 | [Lab 20: Transit Gateway](https://000020.awsstudygroup.com/) |
| 3 | **Cấu hình Transit Gateway**<br>- Tạo Transit Gateway<br>- Tạo Transit Gateway Attachments cho VPC2, VPC3 và VPC4<br>- Xác thực trạng thái kết nối | 12/05/2026 | 12/05/2026 | [Lab 20: Transit Gateway](https://000020.awsstudygroup.com/) |
| 4 | **Cấu hình định tuyến mạng**<br>- Tạo Transit Gateway Route Table<br>- Cập nhật các bảng định tuyến VPC Route Table cho tất cả các VPC được kết nối<br>- Kiểm tra kết nối giữa các VPC | 13/05/2026 | 13/05/2026 | [Lab 20: Transit Gateway](https://000020.awsstudygroup.com/) |
| 5 | **Lab 13 - AWS Backup**<br>- Tạo Amazon S3 bucket<br>- Triển khai hạ tầng sao lưu<br>- Xác thực các tài nguyên cần thiết | 14/05/2026 | 14/05/2026 | [Lab 13: AWS Backup](https://000013.awsstudygroup.com/) |
| 6 | **Cấu hình AWS Backup**<br>- Tạo Backup Plan<br>- Cấu hình các quy tắc sao lưu và policy vòng đời<br>- Cấu hình thông báo sao lưu | 15/05/2026 | 15/05/2026 | [Lab 13: AWS Backup](https://000013.awsstudygroup.com/) |
| 7 | **Xác thực sao lưu và khôi phục**<br>- Thực hiện các công việc sao lưu (backup job)<br>- Khôi phục các tài nguyên được bảo vệ<br>- Xác thực kết quả khôi phục và tính toàn vẹn của bản sao lưu | 16/05/2026 | 16/05/2026 | [Lab 13: AWS Backup](https://000013.awsstudygroup.com/) |

### Kết quả đạt được tuần 4:

* **Thiết kế kiến trúc mạng Hub-and-Spoke**: Triển khai AWS Transit Gateway như một trung tâm định tuyến tập trung kết nối nhiều VPC, giảm độ phức tạp của mạng và cung cấp giải pháp thay thế có khả năng mở rộng tốt hơn so với việc quản lý nhiều kết nối VPC Peering riêng lẻ.
* **Triển khai định tuyến liên VPC tập trung**: Cấu hình các Transit Gateway Attachment và Transit Gateway Route Table, cho phép giao tiếp có kiểm soát giữa các VPC trong khi vẫn duy trì việc quản lý định tuyến đơn giản.
* **Xác thực kết nối đa VPC an toàn**: Cập nhật các bảng định tuyến VPC và xác thực giao tiếp đầu-cuối giữa các instance EC2 trên các VPC được kết nối, đảm bảo lưu lượng truy cập luôn nằm trong mạng riêng của AWS.
* **Xây dựng chiến lược sao lưu tự động**: Cấu hình AWS Backup bằng cách tạo các Backup Plan với quy trình sao lưu theo lịch trình, policy lưu giữ và cấu hình vòng đời để tự động hóa việc bảo vệ dữ liệu.
* **Cấu hình giám sát và thông báo sao lưu**: Kích hoạt các thông báo sao lưu để theo dõi tiến trình thực hiện công việc sao lưu, nâng cao khả năng giám sát vận hành và đảm bảo các tác vụ sao lưu hoàn thành thành công.
* **Xác thực quy trình khôi phục sau sự cố**: Thực hiện các bài kiểm tra khôi phục sao lưu để xác định các điểm phục hồi, xác nhận tính toàn vẹn của dữ liệu và đảm bảo rằng khối lượng công việc có thể được khôi phục thành công trong các tình huống gặp sự cố.
* **Tăng cường tính đàn hồi của cơ sở hạ tầng**: Tích lũy kinh nghiệm thực tế trong triển khai kết nối mạng có tính sẵn sàng cao và giải pháp sao lưu tự động, thiết lập nền tảng vững chắc cho một môi trường AWS an toàn, có thể mở rộng và có khả năng chống chịu sự cố.
