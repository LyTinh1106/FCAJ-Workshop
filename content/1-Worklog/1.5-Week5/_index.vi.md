---
title: "Worklog Tuần 5"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

* Hiểu cách AWS Lambda tự động hóa các tác vụ vận hành để giảm chi phí chạy Amazon EC2.
* Học cách triển khai quản lý tài nguyên bằng cách sử dụng các API của AWS Lambda và Amazon EC2.
* Cấu hình các IAM Role với đặc quyền tối thiểu để cho phép thực thi Lambda an toàn.
* Triển khai môi trường VPC hỗ trợ và cấu hình các Security Group cho các instance EC2.
* Tích hợp AWS Lambda với Slack bằng Incoming Webhook để nhận thông báo cơ sở hạ tầng theo thời gian thực.
* Triển khai tự động hóa dựa trên thẻ (tag) để quản lý chọn lọc các instance EC2 mà không ảnh hưởng đến các tài nguyên khác.
* Xác thực việc quản lý vòng đời instance tự động và giám sát thực thi thông qua AWS CloudWatch log và thông báo Slack.
* Tích lũy kinh nghiệm thực tế trong xây dựng các giải pháp tự động hóa hướng sự kiện (event-driven) giúp nâng cao hiệu quả vận hành và tối ưu hóa chi phí.

### Các công việc cần triển khai trong tuần này:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2| **Lab 22 - Optimizing EC2 Costs with Lambda**<br>- Chuẩn bị tài nguyên <br>- Tạo VPC<br>- Kích hoạt Tự động gán địa chỉ IPv4 công cộng cho các subnet public<br>- Tạo Security Group | 18/05/2026 | 18/05/2026 | [Lab 22: Optimizing EC2 Costs with Lambda](https://000022.awsstudygroup.com/) |
| 3 | **Triển khai tài nguyên máy chủ**<br>- Khởi chạy instance EC2<br>- Cấu hình thẻ (tag) instance EC2 phục vụ tự động hóa<br>- Tạo Slack Workspace và Incoming Webhook | 19/05/2026 | 19/05/2026 | [Lab 22: Optimizing EC2 Costs with Lambda](https://000022.awsstudygroup.com/) |
| 4 | **Cấu hình IAM và Lambda**<br>- Tạo IAM Role phục vụ thực thi Lambda<br>- Gán các quyền quản lý các instance EC2<br>- Xác thực cấu hình IAM Role | 20/05/2026 | 20/05/2026 | [Lab 22: Optimizing EC2 Costs with Lambda](https://000022.awsstudygroup.com/) |
| 5 | **Phát triển các hàm tự động hóa**<br>- Tạo hàm Lambda để dừng các instance EC2<br>- Tạo hàm Lambda để khởi động các instance EC2<br>- Tích hợp logic thông báo qua Slack | 21/05/2026 | 21/05/2026 | [Lab 22: Optimizing EC2 Costs with Lambda](https://000022.awsstudygroup.com/) |
| 6 | **Xác thực quy trình tự động hóa**<br>- Thử nghiệm hoạt động khởi động và dừng tự động<br>- Xác thực log thực thi của Lambda<br>- Xác nhận các thông báo qua Slack và các chuyển đổi trạng thái của EC2 | 22/05/2026 | 22/05/2026 | [Lab 22: Optimizing EC2 Costs with Lambda](https://000022.awsstudygroup.com/) |

### Kết quả đạt được tuần 5:

* **Tự động hóa tối ưu hóa chi phí EC2**: Phát triển các hàm AWS Lambda để tự động khởi động và dừng các instance Amazon EC2 dựa trên yêu cầu vận hành, giảm chi phí máy chủ không cần thiết cho các môi trường thử nghiệm (non-production).
* **Triển khai quản lý tài nguyên dựa trên thẻ (Tag-based)**: Áp dụng các thẻ định danh instance EC2 để xác định mục tiêu tự động hóa, cho phép quản lý tài nguyên có tính chọn lọc và mở rộng mà không ảnh hưởng đến cơ sở hạ tầng không liên quan.
* **Cấu hình phân quyền Serverless an toàn**: Tạo các IAM Role tuân thủ Nguyên tắc đặc quyền tối thiểu, cho phép hàm Lambda quản lý an toàn các instance EC2 trong khi giảm thiểu tối đa các quyền hạn không cần thiết.
* **Xây dựng quy trình tự động hóa hướng sự kiện**: Thiết kế một giải pháp tự động hóa serverless tích hợp hàm AWS Lambda với API của Amazon EC2 để thực hiện các thao tác hạ tầng mà không cần can thiệp thủ công.
* **Tích hợp thông báo vận hành thời gian thực**: Kết nối AWS Lambda với Slack thông qua Incoming Webhook, tự động gửi thông báo mỗi khi các instance EC2 được khởi động hoặc dừng lại.
* **Xác thực tự động hóa đầu-cuối**: Thử nghiệm thành công toàn bộ quy trình tự động hóa bằng cách xác nhận các chuyển đổi trạng thái của EC2, xem lại log thực thi trên CloudWatch và kiểm tra việc gửi nhận thông báo trên Slack.
* **Củng cố kỹ năng vận hành đám mây**: Tích lũy kinh nghiệm thực tế trong công nghệ serverless, tự động hóa hạ tầng, bảo mật IAM và tối ưu hóa chi phí vận hành sử dụng các dịch vụ gốc của AWS và kiến trúc hướng sự kiện.
