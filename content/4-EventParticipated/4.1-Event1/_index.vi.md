---
title: "FCAJ Community Day - Tháng 5 2026"
date: 2026-05-23
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

### Mục Đích Của Sự Kiện

*   Hiểu rõ bản chất và cách thức xây dựng ngữ cảnh (context) để tối ưu hóa hiệu quả của AI.
*   Cập nhật các công cụ AI hỗ trợ phân tích dữ liệu và tự động hóa quy trình làm việc.
*   Nắm bắt giải pháp phân phối nội dung, tối ưu chi phí và bảo mật với nền tảng Cloud.
*   Lắng nghe kinh nghiệm thực chiến từ quá trình xây dựng sản phẩm công nghệ trong môi trường áp lực cao.
*   Khám phá tính chất kỹ thuật cốt lõi của LLM và kiến trúc hệ thống Multi-Agent cấp doanh nghiệp.

### Danh Sách Diễn Giả

*   **Tinh Truong** - Platform Engineer tại GoTymeX.
*   **Pham Ng Hai Anh** - AWS Community Builder tại G-AsiaPacific Vietnam.
*   **Nguyen Tuan Thinh** - DevOps Engineer tại First Cloud AI Journey.
*   **Team đại diện dự án UTMorpho** - Hackathon LotusHacks 2026.
*   **Duc Dao** - Solution Architect tại Cloud Kinetics.
*   **Vy Lam** - Senior Business Systems Analyst tại VPBank.

---

## Nội dung nổi bật từ Sự kiện

### 1. Tối ưu hóa AI với Context & Bộ công cụ Amazon Quick
*   **Context Is Everything & AI-First Mindset:** Xây dựng tư duy ưu tiên AI (AI-first mindset) và đẩy mạnh áp dụng AI (AI adoption) vào công việc thực tế. AI sẽ thất bại nếu thiếu ngữ cảnh (AI context). Việc chuyển dịch từ những câu lệnh (prompts) đơn giản sang khái niệm **"Second AI Brain"** (bộ não AI thứ hai/bộ nhớ dài hạn), kết hợp với các công cụ lấy dữ liệu trực tiếp (**Internet puller**) giúp kết quả đầu ra chính xác, thực tế và mang tính cá nhân hóa cao hơn.
*   **Amazon Quick Ecosystem:**
    *   **Quick Chat Agent:** Trợ lý ảo hỗ trợ khám phá và phân tích dữ liệu.
    *   **Quick Flows & Spaces:** Khởi tạo quy trình tự động bằng ngôn ngữ tự nhiên (không cần code) và chia sẻ không gian làm việc để chuyển hóa insight cá nhân thành tri thức chung của team.
    *   **Quick Sight:** Tự động hóa việc xây dựng dashboard từ dữ liệu thô.
    *   *Điểm nhấn:* Người dùng có thể dễ dàng tiếp cận hệ sinh thái này vì nó hỗ trợ **miễn phí trên phiên bản máy tính (Free on desktop version)**.

### 2. Nền tảng hạ tầng với AWS CloudFront
*   Tổng quan về giải pháp phân phối nội dung (Edge to Origin) phù hợp cho mọi loại workload.
*   Đi sâu vào 4 trụ cột quan trọng: Tối ưu chi phí, Năng lực bảo mật, Tăng cường độ tin cậy (reliability) và Tối ưu hóa hiệu năng hệ thống với hạ tầng AWS CloudFront.

### 3. Hành trình thực chiến & Kiến trúc LLM/AI chuyên sâu
*   **36 giờ cùng LotusHacks:** Quá trình lên ý tưởng, định hình vấn đề, vượt qua các giới hạn và xây dựng sản phẩm UTMorpho trong môi trường hackathon áp lực cao.
*   **Bản chất của "Deterministic" trong LLM:** Đập tan lầm tưởng rằng thiết lập `Temperature = 0` sẽ đảm bảo tính tất định hoàn toàn (Non-Determinism of "Deterministic" LLM Settings). Các cơ chế tối ưu hóa suy luận (inference optimizations) thực tế vẫn mang lại sự ngẫu nhiên và cần có chiến lược giảm thiểu rủi ro (mitigation strategies).
*   **Enterprise-Grade Multi-Agent System:**
    *   Phân tích sự chênh lệch cấu trúc giữa dữ liệu startup và hệ thống ngân hàng truyền thống (Case study: Chấm điểm tín dụng).
    *   Khung kiến trúc (Blueprint) của một hội đồng tín dụng ảo sử dụng mô hình Đa tác vụ (**Multi Agent Paradigm**).
    *   Các nguyên tắc về Guardrails, tuân thủ (Compliance) và đo lường ROI khi triển khai.

---

## Bài học và Định hướng ứng dụng

### Những gì học được
*   **Tư duy Ứng dụng AI:** Hiểu chất lượng đầu vào quyết định đầu ra và tầm quan trọng của việc nạp đúng "AI context", xây dựng bộ nhớ phụ trợ (Second AI Brain). Đồng thời, nắm rõ ranh giới khi nào dùng Single Agent và khi nào bắt buộc nâng cấp lên Multi-Agent để giải quyết bài toán phức tạp.
*   **Kiến trúc & Công nghệ Cốt lõi:**
    *   **Giao thức ngữ cảnh mô hình (MCP):** Mở rộng kiến thức về **MCP guide** và kỹ thuật **MCP attach vector** để kết nối LLM với các nguồn dữ liệu bên ngoài (như cơ sở dữ liệu vector), cung cấp ngữ cảnh động phong phú.
    *   **Cơ chế LLM chuyên sâu:** Nhận thức rõ cách LLM chọn token tiếp theo và tác động của tối ưu hóa suy luận đến độ ổn định hệ thống.
    *   **Hạ tầng mạng:** Củng cố tư duy thiết kế hệ thống phân tán từ Edge đến Origin bằng AWS CloudFront.

### Định hướng ứng dụng vào công việc
*   **Tối ưu hóa Backend:** Tích hợp AWS CloudFront vào các dự án hiện tại (như hệ thống Video-on-Demand hoặc thương mại điện tử) để tăng tốc độ truyền tải nội dung tĩnh.
*   **Nâng cao hiệu suất nhóm:** Đề xuất và thử nghiệm Amazon Quick Flows để tự động hóa quy trình làm việc của nhóm nhờ tính năng miễn phí trên máy tính (**Free on desktop version**).
*   **Thiết kế AI an toàn & mở rộng:** Áp dụng các khái niệm về **Multi Agent**, tích hợp **MCP attach vector** để tối ưu hóa context cho AI, và thiết lập Guardrails an toàn trong các đồ án chuyên ngành Kỹ thuật Phần mềm.
*   **Phát triển bản thân:** Định hình tư duy **AI-first mindset**, sẵn sàng tăng cường mức độ thích ứng công nghệ AI (**AI adoption**) nhằm tạo lợi thế cạnh tranh lớn tại bootcamp.

---

## Trải nghiệm và Ấn tượng cá nhân

Bắt đầu buổi sáng từ tầng 26, sự kiện thực sự đã mang lại một không gian chia sẻ kiến thức công nghệ chuyên sâu và tràn đầy cảm hứng.

*   **Đa dạng về chuyên môn:** Các chủ đề được thiết kế nối tiếp nhau rất logic, dẫn dắt từ cách sử dụng AI hàng ngày, hạ tầng AWS CloudFront vững chắc, cho đến những bài toán học thuật và doanh nghiệp phức tạp như Multi-Agent hay tính Non-Determinism trong LLM.
*   **Góc nhìn thực tế:** Phần trình bày của đội ngũ LotusHacks về hành trình 36 giờ xây dựng UTMorpho mang lại cảm giác rất gần gũi và thực tế. Nó truyền động lực to lớn về cách triển khai ý tưởng nhanh chóng và chấp nhận rủi ro để hoàn thiện sản phẩm.
*   **Nâng tầm tư duy kỹ thuật:** Buổi workshop giúp tôi thoát khỏi tư duy sử dụng các công cụ một cách bề mặt. Việc hiểu được tại sao `Temperature=0` vẫn chưa đủ để kiểm soát LLM hoàn toàn đã thay đổi cách tôi sẽ cấu hình và tích hợp các model vào hệ thống thực tế sau này.

### Một số hình ảnh khi tham gia sự kiện

![Check-in on the 26th floor](/images/4-eventparticipated/event1-1.jpg)
![Check-in on the 26th floor](/images/4-eventparticipated/event1-2.jpg)

> Tổng thể, sự kiện không chỉ là nơi cập nhật các xu hướng công nghệ mới nhất mà còn trang bị cho tôi những phương pháp luận thực tế, vững chắc để tự tin xây dựng, tối ưu hóa và tích hợp AI vào các ứng dụng hiện đại.