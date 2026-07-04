---
title: "Worklog Tuần 10"
date: 2026-07-03
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---


### Mục tiêu tuần 10:

* Tích hợp dịch vụ định danh Amazon Cognito vào giao diện web AWS Amplify để quản lý đăng nhập và xác thực người dùng.
* Cấu hình Amazon S3 bucket để làm kho lưu trữ tệp tin CV tải lên của người dùng.
* Phát triển các hàm AWS Lambda thực hiện chức năng tải lên (upload) và liệt kê (list) các tệp CV từ S3 bucket.
* Thiết lập các endpoint trên API Gateway để tích hợp và bảo mật các luồng xử lý CV từ frontend.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 8 | **Tích hợp Cognito vào giao diện Amplify và test**<br>- Tích hợp thư viện AWS Amplify SDK vào giao diện web frontend<br>- Xây dựng giao diện đăng ký, đăng nhập và xác thực OTP/email sử dụng Cognito User Pool<br>- Kiểm tra luồng xác thực người dùng, bảo mật các router chỉ cho phép người dùng đã đăng nhập truy cập. | 21/06/2026 | 24/06/2026 | |
| 2 | **Cấu hình S3 lưu trữ CV**<br>- Khởi tạo Amazon S3 Bucket chuyên dụng làm kho lưu trữ tệp CV tải lên của ứng viên<br>- Cấu hình policy bảo mật cho bucket (Bucket Policy), chặn truy cập public mặc định<br>- Thiết lập CORS cho S3 để cho phép tải trực tiếp tệp lên từ trình duyệt web. | 22/06/2026 | 22/06/2026 | |
| 2 | **Tạo Lambda upload CV và list CV từ S3**<br>- Viết mã nguồn Lambda tạo presigned URL cho phép frontend upload trực tiếp CV lên S3 an toàn<br>- Viết mã nguồn Lambda thực hiện quét và lấy danh sách các CV hiện có trong bucket của người dùng cụ thể<br>- Cấu hình quyền IAM cho các hàm Lambda truy cập tài nguyên S3. | 22/06/2026 | 23/06/2026 | |
| 5 | **Tạo API endpoint cho Lambda upload CV và list CV**<br>- Cấu hình các route mới trên API Gateway kết nối với các hàm Lambda upload và list CV<br>- Tích hợp bộ xác thực Cognito Authorizer trên API Gateway để bảo vệ các endpoint này<br>- Thử nghiệm gọi API từ frontend và xác thực việc upload/list dữ liệu tệp tin. | 25/06/2026 | 27/06/2026 | |


### Kết quả đạt được tuần 10:

* **Tích hợp xác thực người dùng**: Tích hợp và thử nghiệm thành công chức năng đăng nhập, đăng ký bằng Amazon Cognito trên giao diện Amplify.
* **Quản lý lưu trữ tài liệu**: Khởi tạo và cấu hình phân quyền bảo mật cho S3 bucket lưu trữ CV của người dùng an toàn.
* **Xây dựng chức năng xử lý tệp tin**: Xây dựng hoàn tất các hàm Lambda xử lý upload CV lên S3 và lấy danh sách CV đã upload.
* **Kết nối API frontend-backend**: Triển khai thành công các API endpoint kết nối frontend với backend phục vụ cho luồng nghiệp vụ quản lý CV.
