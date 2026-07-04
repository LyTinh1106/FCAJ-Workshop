---
title: "Worklog Tuần 7"
date: 2026-07-03
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Làm chủ việc kiểm soát truy cập nâng cao trong AWS Identity and Access Management (IAM) sử dụng Thẻ tài nguyên (Resource Tags) và policy (Policies).
* Cấu hình Điều kiện của IAM Role (IAM Role Conditions) để giới hạn việc giả định vai trò (role-assumption) theo địa chỉ IP và khoảng thời gian cụ thể.
* Ủy quyền cho các ứng dụng trên Amazon EC2 truy cập an toàn vào Amazon S3 bucket sử dụng IAM Role.

### Các công việc cần triển khai trong tuần này:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Lab 28: Quản lý quyền truy cập dịch vụ EC2 bằng Thẻ tài nguyên thông qua dịch vụ IAM** <br>- Tạo IAM user mới cho bài lab <br>- Tạo policy IAM tùy chỉnh và IAM role <br>- Xác thực áp dụng policy trên IAM user: <br>&emsp; + Chuyển đổi vai trò (Switch role) <br>&emsp; + Thử nghiệm truy cập EC2 console theo vùng: Tokyo (bị từ chối) vs. N. Virginia (được cho phép) <br>&emsp; + Xác thực các quy tắc tạo EC2 (không thẻ vs. có thẻ phù hợp) <br>&emsp; + Thử nghiệm chỉnh sửa Thẻ tài nguyên trên instance EC2 (bị từ chối bởi policy) | 01/06/2026 | 01/06/2026      | [Lab 28: Manage Access to EC2 Services with Resource Tags through IAM Services](https://000028.awsstudygroup.com/) |
| 3 | **Lab 44: IAM Role & Condition** <br>- Tạo nhóm IAM và các người dùng IAM <br>- Xác thực các quyền mặc định của người dùng <br>- Cấu hình IAM Admin Role và các tham số switch role <br>- Áp dụng điều kiện để giới hạn quyền switch role: <br>&emsp; + Giới hạn switch role theo địa chỉ IP cụ thể <br>&emsp; + Giới hạn switch role theo khung thời gian cụ thể | 02/06/2026 | 02/06/2026      | [Lab 44: IAM Role & Condition](https://000044.awsstudygroup.com/) |
| 4 | **Lab 48: Cấp quyền cho ứng dụng truy cập dịch vụ AWS bằng IAM Role** <br>- Triển khai môi trường: khởi chạy instance EC2 và tạo một S3 bucket <br>- Tạo một IAM user cụ thể và kích hoạt access key <br>- Tạo một IAM role để cấp quyền truy cập S3 an toàn bằng thông tin xác thực tạm thời thông qua access key | 04/06/2026 | 04/06/2026      | [Lab 48: Granting Authorization for Application to Access AWS Services with IAM Role](https://000048.awsstudygroup.com/) |


### Kết quả đạt được tuần 7:

* **Triển khai kiểm soát truy cập dựa trên thuộc tính (ABAC)**: Thực thi ranh giới truy cập nghiêm ngặt trên các instance EC2 bằng cách sử dụng các khóa điều kiện trong policy IAM khớp với thẻ tài nguyên.
* **Kiểm soát truy cập cấp vùng (Region-level)**: Xác thực các policy IAM giới hạn giao diện điều khiển dịch vụ giữa các vùng, cho phép thực hiện thành công các hoạt động tại vùng `us-east-1` (North Virginia) trong khi chặn quyền truy cập tại vùng `ap-northeast-1` (Tokyo).
* **Áp dụng điều kiện policy IAM nâng cao**: Giới hạn đặc quyền giả định vai trò quản trị (administrative role-assumption) bằng cách kết hợp các quy tắc điều kiện đa yếu tố (giới hạn địa chỉ IP và giới hạn thời gian thực thi).
* **Quản lý ủy quyền từ ứng dụng đến dịch vụ (App-to-Service)**: Cho phép truy cập lập trình an toàn và tiêu chuẩn vào các tài nguyên S3 từ các node tính toán mà không cần nhúng thông tin xác thực tĩnh (secret credentials) trực tiếp vào mã nguồn hoặc các instance.
