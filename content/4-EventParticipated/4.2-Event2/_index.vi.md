---
title: "Event Meet up 06-06-2026"
date: 2026-06-06
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---
### Mục Đích Của Sự Kiện

*   Chia sẻ kinh nghiệm thực tiễn và bài học đắt giá trong quá trình học tập, tự nghiên cứu cũng như phát triển dự án công nghệ đám mây và AI.
*   Trao đổi kiến thức chuyên sâu về công nghệ container hóa, lập trình kết nối thời gian thực, hệ thống phát hiện xâm nhập và giải pháp GraphRAG hiện đại.
*   Lan tỏa tinh thần làm việc nhóm hiệu quả, định hình tư duy thiết kế hệ thống và xây dựng lộ trình nâng cấp bản thân từ vị trí khởi điểm lên chuyên gia.

### Danh Sách Diễn Giả

*   **Nguyễn Quốc Bảo** - Godot Client & AWS WebSockets.
*   **Bảo Huỳnh** - Công nghệ Container hóa với Docker.
*   **Việt Phát** - Giải pháp GraphRAG với Bedrock & Neptune.
*   **Lê Hoàng Gia Đại** - NIDS dựa trên Machine Learning.
*   **Trương Huy Phước** - Nghệ thuật làm việc nhóm hiệu quả.
*   **Trần Trung Vinh** - Hành trình từ IT Helpdesk đến Senior Sysadmin.

---

## Nội dung nổi bật từ Sự kiện

### 1. Kết nối Godot Client với AWS WebSockets cho Game Multiplayer (Bảo Nguyễn)
*   **Kiến trúc Serverless kết nối hai chiều**: Tận dụng AWS API Gateway WebSocket để duy trì kết nối bền vững với độ trễ tối thiểu, kết hợp AWS Lambda xử lý logic và Amazon DynamoDB lưu trữ trạng thái trận đấu.
*   **Tích hợp sâu trong Engine Godot**: Cấu hình chi tiết lớp `WebSocketPeer` và tối ưu hóa vòng lặp `_process` để đảm bảo đồng bộ hóa thông tin và phản hồi mạng theo thời gian thực.
*   **Giải quyết bài toán thực tế**: Đưa ra giải pháp tối ưu hóa chi phí đọc/ghi DynamoDB và dọn dẹp các kết nối "stale" (ngắt vật lý nhưng vẫn tồn tại trên cơ sở dữ liệu) nhằm tránh hao phí tài nguyên.

### 2. Công nghệ Container hóa với Docker (Bảo Huỳnh)
*   **Giải pháp đóng gói toàn diện**: Đóng gói ứng dụng cùng toàn bộ thư viện, cấu hình và thành phần phụ thuộc vào một Docker Image duy nhất để giải quyết triệt để vấn đề không nhất quán môi trường ("chạy được ở local nhưng lỗi trên production").
*   **Tối ưu hóa tài nguyên phần cứng**: Khác với ảo hóa truyền thống chạy OS khách đầy đủ, Docker chia sẻ nhân OS máy chủ giúp khởi động container nhanh chóng trong vài giây và tiết kiệm RAM/CPU.
*   **Đẩy mạnh chu kỳ CI/CD & Microservices**: Hỗ trợ tăng tốc độ phát triển và triển khai tự động qua ba thành phần cốt lõi: Dockerfile (chỉ dẫn build), Docker Image (khuôn mẫu tĩnh) và Docker Container (thực thể đang chạy).

### 3. Giải pháp GraphRAG với Amazon Bedrock và Neptune (Việt Phát)
*   **Khắc phục giới hạn RAG truyền thống**: Sử dụng đồ thị tri thức (Knowledge Graph) để thực hiện suy luận đa bước (multi-hop reasoning) phức tạp và phân tích trực quan mối quan hệ giữa các thực thể thông tin.
*   **Lộ trình triển khai linh hoạt**:
    *   **Fully Managed**: Tận dụng Amazon Bedrock Knowledge Bases tích hợp sẵn với Neptune Analytics giúp rút ngắn thời gian phát triển.
    *   **Custom**: Sử dụng LlamaIndex xây dựng pipeline dữ liệu tùy chỉnh, cho phép truy vấn trực tiếp bằng ngôn ngữ Cypher trên Amazon Neptune nhằm đạt độ tùy biến tối đa.

### 4. Hệ thống phát hiện xâm nhập (NIDS) dựa trên Machine Learning (Đại Lê)
*   **Giải pháp bảo mật kết hợp đột phá**: Tích hợp AWS WAF (luật tĩnh) với Machine Learning để phát hiện hiệu quả các cuộc tấn công Zero-day và hành vi xâm nhập dị thường mà tường lửa thông thường bỏ sót.
*   **Quy trình huấn luyện mô hình chuẩn**: Sử dụng tập dữ liệu CSE-CIC-IDS2018 để huấn luyện mô hình phân loại chính xác các đòn tấn công mạng phổ biến như Botnet, DoS, DDoS và Brute Force.
*   **Tối ưu hóa khả năng nhận diện**: Áp dụng kỹ thuật xử lý dữ liệu mất cân bằng nhằm tăng độ nhạy đối với các lớp tấn công thiểu số và tích hợp bảng điều khiển giám sát trực quan thời gian thực.

### 5. Nghệ thuật làm việc nhóm hiệu quả (Trương Phước)
*   **4 Quy tắc vàng nâng tầm phối hợp**: Thiết lập mục tiêu chung thống nhất từ đầu, đặt đúng người vào đúng vị trí theo thế mạnh, giao tiếp cởi mở xây dựng và đề cao tinh thần chịu trách nhiệm.
*   **Cộng hưởng hiệu suất tập thể**: Áp dụng triết lý "nhiều tay thì việc nhẹ" giúp chia sẻ gánh nặng công việc, tối ưu hóa năng lực cá nhân và xóa bỏ rào cản giao tiếp.
*   **Ứng dụng bộ công cụ số**: Khuyên dùng Trello để quản lý tiến độ trực quan, Slack & Discord để thảo luận nhanh và Google Workspace để đồng thiết lập tài liệu một cách linh hoạt.

### 6. Hành trình từ IT Helpdesk đến Senior Sysadmin (Vinh Trần)
*   **Lộ trình tự học và tích lũy thực tế**: Chia sẻ chặng đường nỗ lực bền bỉ đi từ kỹ thuật viên hỗ trợ sơ cấp (Helpdesk) lên chuyên gia hệ thống lớn, dịch chuyển tiếp sang mảng Cloud và DevOps.
*   **Thay đổi tư duy cốt lõi**: Chuyển dịch từ thế bị động sửa lỗi sang chủ động tìm hiểu cấu trúc sâu sắc của hệ thống; khuyên học sâu Linux, Giao thức mạng và tích cực tự dựng lab.
*   **Nguyên tắc Sysadmin bất di bất dịch**: Luôn khắc ghi triết lý bảo vệ hệ thống: "không bao giờ thử nghiệm hoặc debug trực tiếp trên môi trường đang vận hành (Production)".

---

## Bài học và Định hướng ứng dụng

### Những gì học được
*   **Tư duy công nghệ & Bảo mật:** Hiểu rõ giá trị của container hóa với Docker, cơ chế giao tiếp hai chiều real-time qua WebSockets trong game, ứng dụng ML vào việc phát hiện xâm nhập trái phép, và sức mạnh liên kết thực thể của GraphRAG.
*   **Kỹ năng phối hợp & Phát triển:** Nắm vững 4 quy tắc vàng trong làm việc nhóm để vận dụng vào các dự án chung, đồng thời định hình rõ tư duy tự học thực chất để phát triển lộ trình sự nghiệp vững chắc.

### Định hướng ứng dụng vào công việc
*   **Đóng gói container:** Áp dụng Docker vào các đồ án hiện tại để đồng nhất môi trường phát triển và phân phối ứng dụng nhanh chóng.
*   **Thử nghiệm Real-time & AI:** Nghiên cứu tích hợp WebSocket API của API Gateway cho các ứng dụng cần cập nhật trạng thái liên tục và tìm hiểu sâu hơn về GraphRAG với Amazon Bedrock.
*   **Quản trị và Vận hành:** Áp dụng các quy tắc làm việc nhóm và công cụ số như Slack/Trello vào quản lý tiến độ bài tập lớn trong bootcamp, tuân thủ kỷ luật vận hành hệ thống.

---

## Trải nghiệm và Ấn tượng cá nhân

Buổi meetup thực sự đã mang lại một không gian kết nối và trao đổi kiến thức vô cùng năng động và bổ ích:

*   **Sự đa dạng về chủ đề:** Các bài chia sẻ bao phủ từ cơ sở hạ tầng, lập trình game, an toàn thông tin cho đến kỹ năng mềm và câu chuyện phát triển bản thân.
*   **Tính thực chiến cao:** Trải nghiệm từ diễn giả Vinh Trần hay giải pháp thực tế của các diễn giả khác giúp mở rộng góc nhìn và tạo động lực tự học lớn cho các thành viên tham gia.

### Một số hình ảnh khi tham gia sự kiện

![Check-in at the event](/images/4-EventParticipated/event2.jpg)

> Tổng thể, sự kiện đã mang lại cho tôi những kiến thức công nghệ hiện đại và những bài học nghề nghiệp vô cùng giá trị để vững bước hơn trên con đường DevOps/Sysadmin.
