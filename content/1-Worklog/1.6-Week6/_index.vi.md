---
title: "Worklog Tuần 6"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---
### Mục tiêu tuần 6:

* Cài đặt AWS CLI và cấu hình token tài khoản IAM cùng các biến môi trường.
* Hiểu và kích hoạt AWS Security Hub để đánh giá mức độ tuân thủ và trạng thái bảo mật.
* Triển khai chiến lược gắn thẻ (tagging) có cấu trúc trên tài nguyên AWS thông qua Management Console và AWS CLI.
* Phân nhóm và quản lý các tài nguyên sử dụng AWS Resource Groups.

### Các công việc cần triển khai trong tuần này:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Cài đặt & Cấu hình AWS CLI** <br>- Cài đặt AWS CLI <br>- Cấu hình token tài khoản IAM và các biến môi trường | 25/05/2026 | 25/05/2026      | [Lab 11: Getting Started with the AWS CLI](https://000011.awsstudygroup.com/)   |
| 3 | **Lab 18: Security Hub** <br>- Kích hoạt AWS Security Hub <br>- Xem xét các tiêu chuẩn bảo mật và đánh giá điểm số bảo mật dựa trên các chỉ số chuẩn về tuân thủ | 26/05/2026 | 26/05/2026      | [Lab 18: Getting Started with AWS Security Hub](https://000018.awsstudygroup.com/) |
| 4 | **Lab 27: Quản lý tài nguyên bằng Thẻ và Nhóm tài nguyên** <br>- **Gắn thẻ qua AWS Management Console**:<br>&emsp; + Tạo EC2 Instance kèm thẻ<br>&emsp; + Quản lý thẻ EC2 với AWS Resource Groups<br>&emsp; + Lọc tài nguyên bằng thẻ<br>- **Gắn thẻ qua AWS CLI**:<br>&emsp; + Triển khai quản lý tài nguyên dựa trên thẻ bằng các lệnh AWS CLI<br>- **AWS Resource Groups**:<br>&emsp; + Tạo nhóm tài nguyên để tổ chức và quản lý các tài nguyên AWS | 27/05/2026 | 29/05/2026      | [Lab 27: Manage Resources Using Tags and Resource Groups](https://000027.awsstudygroup.com/) |


### Kết quả đạt được tuần 6:

* **Cấu hình môi trường dòng lệnh cục bộ**: Cài đặt thành công AWS Command Line Interface (CLI) để giao tiếp trực tiếp với các dịch vụ AWS.
* **Bảo mật ngữ cảnh xác thực cục bộ**: Cấu hình các session token, access key của IAM và các biến môi trường trên hệ thống cục bộ để xác thực API an toàn.
* **Quản lý trạng thái bảo mật tập trung**: Kích hoạt AWS Security Hub để liên tục giám sát và đánh giá trạng thái bảo mật trên các tài khoản AWS.
* **Đánh giá các tiêu chuẩn bảo mật**: Xem xét điểm số bảo mật tổng thể và các phát hiện (finding) đối với các tiêu chuẩn tuân thủ được hỗ trợ trong ngành (ví dụ: Thực hành bảo mật tốt nhất nền tảng của AWS, CIS Benchmarks).
* **Triển khai chiến lược gắn thẻ chuẩn hóa**: Áp dụng gắn thẻ siêu dữ liệu (metadata tagging) nhất quán trên các instance EC2 và các tài nguyên khác thông qua cả AWS Management Console và AWS CLI.
* **Tối ưu hóa tìm kiếm tài nguyên**: Cấu hình bộ lọc tài nguyên dựa trên các khóa và giá trị thẻ để nhanh chóng tìm thấy các khối lượng công việc và môi trường cụ thể.
* **Tổ chức tài nguyên với Resource Groups**: Tạo và cấu hình thành công các AWS Resource Groups để đơn giản hóa các thao tác hàng loạt, theo dõi và tổ chức các tài nguyên liên quan.
