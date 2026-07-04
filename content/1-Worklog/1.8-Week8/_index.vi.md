---
title: "Worklog Tuần 8"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

* Hiểu kiến trúc và quy trình triển khai dịch vụ cơ sở dữ liệu quan hệ Amazon (Amazon RDS) đối với các cơ sở dữ liệu quan hệ được quản lý.
* Học cách kết nối an toàn các ứng dụng trên Amazon EC2 tới Amazon RDS sử dụng mạng VPC và các Security Group.
* Cấu hình các cơ chế sao lưu, snapshot và khôi phục cơ sở dữ liệu để cải thiện độ bền dữ liệu và tính sẵn sàng khôi phục sau sự cố.
* Khám phá các khái niệm cốt lõi của cơ sở dữ liệu NoSQL thông qua Amazon DynamoDB, bao gồm bảng, mục (item), thuộc tính (attribute) và khóa chính (primary key).
* Thực hiện các thao tác CRUD trên Amazon DynamoDB bằng cách sử dụng AWS Management Console, AWS CloudShell và AWS CLI.
* Tích hợp ứng dụng Python với Amazon DynamoDB sử dụng bộ phát triển phần mềm AWS SDK (Boto3) để thực hiện các thao tác cơ sở dữ liệu bằng lập trình.
* So sánh các mô hình cơ sở dữ liệu quan hệ và NoSQL, xác định các trường hợp sử dụng phù hợp cho Amazon RDS và Amazon DynamoDB.
* Tích lũy kinh nghiệm thực tế trong triển khai, quản lý và tích hợp các dịch vụ cơ sở dữ liệu được quản lý bởi AWS vào các ứng dụng cloud-native.

### Các công việc cần triển khai trong tuần này:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Lab 05 - Amazon Relational Database Service (Amazon RDS)** <br> - Chuẩn bị tài nguyên <br> - Tạo VPC<br>- Tạo EC2 Security Group<br>- Tạo RDS Security Group<br>- Tạo DB Subnet Group | 08/06/2026 | 08/06/2026 | [Lab 05: Amazon Relational Database Service (Amazon RDS)](https://000005.awsstudygroup.com/) |
| 3 | **Triển khai Amazon RDS**<br>- Khởi chạy instance EC2<br>- Tạo instance DB Amazon RDS<br>- Cấu hình kết nối giữa EC2 và RDS | 09/06/2026 | 09/06/2026 | [Lab 05: Amazon Relational Database Service (Amazon RDS)](https://000005.awsstudygroup.com/) |
| 4 | **Xác thực triển khai RDS**<br>- Triển khai ứng dụng kết nối tới Amazon RDS<br>- Kiểm tra các thao tác cơ sở dữ liệu<br>- Thực hiện xác thực sao lưu và khôi phục | 10/06/2026 | 10/06/2026 | [Lab 05: Amazon Relational Database Service (Amazon RDS)](https://000005.awsstudygroup.com/) |
| 6 | **Lab 60 - DynamoDB Fundamentals**<br>- Tạo các bảng DynamoDB<br>- Thực hiện các thao tác CRUD bằng AWS Management Console<br>- Thực hiện các thao tác DynamoDB qua AWS CloudShell<br>- Cấu hình thông tin xác thực AWS CLI | 12/06/2026 | 12/06/2026 | [Lab 60: Work with Amazon DynamoDB](https://000060.awsstudygroup.com/) |
| 7 | **Tích hợp DynamoDB vào ứng dụng**<br>- Cấu hình AWS SDK (Boto3)<br>- Tích hợp DynamoDB vào một ứng dụng Python<br>- Xác thực các thao tác cơ sở dữ liệu ở cấp độ ứng dụng | 13/06/2026 | 13/06/2026 | [Lab 60: Work with Amazon DynamoDB](https://000060.awsstudygroup.com/) |

### Kết quả đạt được tuần 8:

* **Triển khai hạ tầng cơ sở dữ liệu quan hệ an toàn**: Xây dựng môi trường Amazon RDS bằng cách cấu hình mạng VPC, Security Group và DB Subnet Group, đảm bảo giao tiếp an toàn giữa các tầng ứng dụng và cơ sở dữ liệu.
* **Tích hợp ứng dụng với Amazon RDS**: Triển khai thành công ứng dụng web trên Amazon EC2 và thiết lập kết nối tin cậy đến cơ sở dữ liệu Amazon RDS để lưu trữ và truy xuất dữ liệu.
* **Triển khai sao lưu và khôi phục cơ sở dữ liệu**: Tạo các bản snapshot cơ sở dữ liệu và xác thực quy trình khôi phục, chứng minh khả năng bảo vệ và phục hồi các cơ sở dữ liệu quan hệ được quản lý.
* **Phát triển kỹ năng cơ sở dữ liệu NoSQL thực tế**: Tạo các bảng DynamoDB, quản lý các mục dữ liệu và thực hiện các thao tác CRUD sử dụng AWS Management Console, AWS CloudShell và AWS CLI.
* **Xây dựng tích hợp cơ sở dữ liệu bằng lập trình**: Cấu hình bộ phát triển phần mềm AWS SDK (Boto3) và thông tin xác thực AWS CLI để cho phép ứng dụng Python tương tác với Amazon DynamoDB thông qua các hoạt động dựa trên API.
* **So sánh các mô hình cơ sở dữ liệu quan hệ và NoSQL**: Đạt được hiểu biết thực tế về sự khác biệt giữa Amazon RDS và Amazon DynamoDB, bao gồm mô hình dữ liệu, đặc tính mở rộng và các tình huống ứng dụng phù hợp.
* **Nâng cao chuyên môn quản lý dữ liệu trên AWS**: Tích lũy kinh nghiệm thực tế trong triển khai, quản lý, bảo mật và tích hợp các dịch vụ cơ sở dữ liệu được quản lý bởi AWS, tạo nền tảng vững chắc cho việc phát triển các ứng dụng hướng dữ liệu cloud-native.
