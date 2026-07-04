---
title: "Worklog Tuần 11"
date: 2026-07-03
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---


### Mục tiêu tuần 11:

* Nghiên cứu và tìm hiểu dịch vụ trích xuất văn bản tự động Amazon Textract.
* Triển khai giải pháp sử dụng Amazon Textract để xử lý và trích xuất nội dung văn bản từ các tệp CV định dạng PDF.
* Tích hợp trí tuệ nhân tạo (AI/LLM) để phân tích, đánh giá nội dung CV dựa trên các yêu cầu công việc.
* Hoàn thiện tài liệu nhật ký công việc (worklog) và báo cáo tiến độ dự án.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | **Tìm hiểu về Textract**<br>- Đọc tài liệu kỹ thuật về Amazon Textract và các API hỗ trợ trích xuất văn bản từ tài liệu quét/hình ảnh/PDF<br>- Thử nghiệm trích xuất thử nghiệm trên AWS Console để hiểu cấu trúc JSON trả về (Blocks, Lines, Words). | 29/06/2026 | 29/06/2026 | |
| 2 | **Triển khai Textract để xử lý nội dung từ file PDF**<br>- Phát triển hàm Lambda tích hợp thư viện Boto3 để gọi Amazon Textract xử lý các tệp PDF lưu trên S3<br>- Xây dựng thuật toán phân tích, tổng hợp văn bản từ kết quả trích xuất của Textract để thu về nội dung dạng text thuần túy<br>- Tối ưu hóa xử lý bất đồng bộ (asynchronous) đối với các file PDF nhiều trang. | 29/06/2026 | 30/06/2026 | |
| 4 | **Tích hợp AI để đánh giá CV**<br>- Tích hợp dịch vụ AI (dùng Gemini 3.1 Flash) để phân tích nội dung text của CV<br>- Xây dựng prompt chất lượng cao gửi tới AI để so sánh kỹ năng trong CV với mô tả công việc (Job Description)<br>- Xử lý kết quả trả về từ AI để chấm điểm độ phù hợp và đưa ra nhận xét chi tiết. | 01/07/2026 | 02/07/2026 | |
| 5 | **Viết worklog**<br>- Biên soạn chi tiết báo cáo tiến độ và nhật ký công việc từ tuần 9 đến tuần 11<br>- Đồng bộ và kiểm tra hiển thị nội dung trên giao diện web Hugo để đảm bảo hiển thị đúng định dạng markdown. | 02/07/2026 | 03/07/2026 | |


### Kết quả đạt được tuần 11:

* **Nghiên cứu công nghệ trích xuất**: Nắm vững nguyên lý hoạt động và cách sử dụng Amazon Textract để xử lý tài liệu.
* **Xây dựng luồng trích xuất dữ liệu**: Xây dựng thành công luồng xử lý trích xuất văn bản tự động từ file PDF của CV với độ chính xác cao.
* **Tích hợp trí tuệ nhân tạo**: Tích hợp thành công tính năng AI đánh giá CV giúp tự động nhận diện kỹ năng và độ phù hợp của ứng viên.
* **Hoàn thiện tài liệu hóa**: Cập nhật đầy đủ và chi tiết nhật ký công việc (worklog) cho các tuần triển khai dự án.
