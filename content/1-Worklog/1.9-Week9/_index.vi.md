---
title: "Worklog Tuần 9"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---



### Mục tiêu tuần 9:

* Xây dựng hệ thống tự động thu thập (fetch) dữ liệu công việc (Jobs) qua API sử dụng Amazon EventBridge/Scheduler.
* Triển khai hosting giao diện ứng dụng web trên AWS Amplify.
* Thiết kế cơ sở dữ liệu DynamoDB và xây dựng các hàm AWS Lambda để xử lý và lưu trữ thông tin công việc.
* Cấu hình API Gateway để làm cổng kết nối bảo mật cho các dịch vụ backend.
* Quản lý các khóa bí mật (API Keys) một cách an toàn bằng AWS Systems Manager Parameter Store.
* Tìm hiểu dịch vụ quản lý định danh Amazon Cognito và cấu hình Cognito User Pool.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | **Tạo schedule để tự động fetch API**<br>- Nghiên cứu và tìm hiểu về Amazon EventBridge (Scheduler)<br>- Thiết lập quy tắc/lịch trình (cron expression) chạy định kỳ hằng ngày để tự động gọi API lấy thông tin dữ liệu Jobs mới nhất<br>- Kiểm tra log execution để đảm bảo scheduler kích hoạt đúng giờ. | 15/06/2026 | 15/06/2026 | |
| 3 | **Hosting giao diện bằng Amplify**<br>- Cấu hình dự án frontend trên AWS Amplify Console<br>- Kết nối repository chứa mã nguồn frontend (GitHub/GitLab)<br>- Thiết lập quy trình CI/CD tự động build và deploy mỗi khi có thay đổi mã nguồn<br>- Cấu hình domain và kiểm tra khả năng truy cập ứng dụng. | 16/06/2026 | 16/06/2026 | |
| 5 | **Xây dựng Lambda Function và DynamoDB Table để lưu Jobs**<br>- Thiết kế cấu trúc bảng dữ liệu (schema) DynamoDB lưu thông tin Jobs, xác định Partition Key và Sort Key phù hợp<br>- Viết mã nguồn Lambda (Python/Node.js) để xử lý định dạng dữ liệu nhận được từ API và ghi vào DynamoDB<br>- Cấu hình IAM Role và Policy cấp quyền cho Lambda ghi dữ liệu vào DynamoDB. | 18/06/2026 | 18/06/2026 | |
| 6 | **Cấu hình API Gateway**<br>- Khởi tạo REST API hoặc HTTP API trên Amazon API Gateway<br>- Cấu hình các tài nguyên (resource) và phương thức (method like POST, GET) kết nối trực tiếp đến Lambda backend<br>- Cấu hình CORS để cho phép ứng dụng frontend gọi API an toàn<br>- Deploy API lên stage và kiểm tra endpoint hoạt động. | 19/06/2026 | 19/06/2026 | |
| 6 | **Cấu hình Parameter Store để lưu API Keys**<br>- Sử dụng AWS Systems Manager Parameter Store lưu trữ bảo mật thông tin nhạy cảm và API Keys<br>- Phân quyền IAM cho Lambda Function truy cập đọc Parameter Store một cách an toàn<br>- Cập nhật mã nguồn Lambda để lấy API Keys động từ Parameter Store thay vì hardcode. | 19/06/2026 | 19/06/2026 | |
| 7 | **Tìm hiểu về Cognito và cấu hình Cognito User Pool**<br>- Nghiên cứu kiến trúc và tính năng quản lý người dùng của Amazon Cognito<br>- Khởi tạo Cognito User Pool và thiết lập các thuộc tính bắt buộc (email, password policy)<br>- Cấu hình App Client và thiết lập luồng xác thực (OAuth, hosted UI). | 20/06/2026 | 20/06/2026 | |


### Kết quả đạt được tuần 9:

* **Tự động hóa luồng thu thập dữ liệu**: Thiết lập thành công lịch trình tự động gọi API định kỳ để cập nhật dữ liệu.
* **Triển khai ứng dụng web**: Hosting thành công giao diện frontend của ứng dụng lên AWS Amplify, đảm bảo khả năng truy cập toàn cầu.
* **Xây dựng serverless backend & cơ sở dữ liệu**: Xây dựng hoàn chỉnh hàm Lambda và bảng DynamoDB để lưu trữ thông tin Jobs ổn định và hiệu quả.
* **Quản trị API bảo mật**: Cấu hình thành công API Gateway làm điểm cuối (endpoint) để frontend tương tác với Lambda backend.
* **Bảo mật thông tin nhạy cảm**: Lưu trữ an toàn các thông tin cấu hình và API Keys thông qua Parameter Store, tăng tính bảo mật cho hệ thống.
* **Thiết lập luồng quản lý định danh**: Cấu hình thành công Cognito User Pool sẵn sàng cho việc tích hợp tính năng đăng ký, đăng nhập người dùng.
