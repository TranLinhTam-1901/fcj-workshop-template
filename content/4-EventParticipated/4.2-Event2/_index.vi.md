---
title: "Event 2"
date: 2026-06-27
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

<!-- {{% notice warning %}}
⚠️ **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn kể cả warning này.
{{% /notice %}} -->

# Bài thu hoạch “FCAJ COMMUNITY DAY”

### Mục Đích Của Sự Kiện

- Cập nhật xu hướng và giải pháp ứng dụng trí tuệ nhân tạo (AI) vào các bài toán thực tế của doanh nghiệp.
- Giới thiệu các nền tảng và đại lý AI (AI Agents) hỗ trợ tự động hóa quy trình vận hành hệ thống, tối ưu chi phí và nâng cao an toàn bảo mật.
- Chia sẻ kinh nghiệm thực tiễn và giải pháp công nghệ nâng cao hiệu suất trong các lĩnh vực chuyên sâu từ Nhân sự (HR), DevOps đến Công nghệ giọng nói.
- Tạo không gian kết nối, thảo luận giữa các chuyên gia, kỹ sư và cộng đồng công nghệ về định hướng phát triển sự nghiệp trong kỷ nguyên AI.

### Danh Sách Diễn Giả

- **Truong Tran** – AI Solution Sales, Noventiq
- **Steve Tran** – CTO/Founder, CloudThinker
- **Trung Vu** – CEO, Revve AI
- **Anh Dang** – Solution Sales, Noventiq
- **Nghi Danh** – AI Engineer, Renova Cloud
- **Kiet Tran** – AI Engineer, AWS Student Builder Group
- **Bao Phan** – Cloud Engineer, Cloud Kinetics
- **Nguyen Nguyen** – Cloud Engineer, Cloud Kinetics
- **Toan Nguyen** – AWS Security Builder

### Nội Dung Nổi Bật

#### 1. Lộ trình sự nghiệp và Hệ thống Vận hành AI (Aigentic Platform)
- **Thị trường việc làm khắc nghiệt:** Doanh nghiệp ngày càng ưu tiên tuyển dụng nhân sự cấp cao (Senior) có kỹ năng sử dụng AI hoặc có khả năng tối ưu tốc độ làm việc vượt trội nhờ công cụ AI.
- **Nền tảng Aigentic:** Giải pháp đột phá hỗ trợ vận hành Cloud tập trung giải quyết triệt để 3 bài toán lớn:
  - Xử lý sự cố (Incident) tự động tính bằng phút.
  - Kiểm soát chất lượng mã nguồn thông qua Code reviews tự động.
  - FinOps giúp tối ưu hóa chi phí sử dụng Cloud với mức độ tự động hóa từ AI gần như 100%.
- **Tư duy Kiến trúc Multi-agent:** Sử dụng kiến trúc đa tác nhân nhằm tối ưu hóa cửa sổ ngữ cảnh (context window) và phân quyền truy cập hệ thống theo vai trò một cách chặt chẽ (RBAC).

#### 2. Giọng nói của AI cho tiếng Việt (Voice AI)
- **Thách thức ngôn ngữ bản địa:** Tiếng Việt thuộc nhóm ngôn ngữ ít tài liệu (low resource), gây ra nhiều rào cản lớn trong việc huấn luyện các mô hình AI.
- **Kiến trúc hệ thống toàn diện:** Ứng dụng luồng xử lý mượt mà từ STT (Chuyển giọng nói thành văn bản) $\rightarrow$ LLM $\rightarrow$ TTS (Chuyển văn bản thành giọng nói) kết hợp tính năng Tool calling để giải quyết các nghiệp vụ phức tạp trực tiếp (ví dụ: khóa thẻ ngân hàng).
- **Xử lý ngữ cảnh thực tế:** Tối ưu hóa AI để nhận diện giới tính nhằm xưng hô phù hợp, đồng thời hiểu sâu sắc ngữ cảnh để biết lúc nào cần ngắt lời hoặc chờ đợi khách hàng suy nghĩ.

#### 3. Đại lý DevOps AI (DevOps Agent)
- **Vấn đề cốt lõi:** Các kỹ sư DevOps hiện nay tiêu tốn quá nhiều thời gian xử lý do các dữ liệu log/trace bị phân mảnh và thiếu tính đồng bộ, trực quan.
- **Quy trình tự động hóa 4 bước:** DevOps Agent chuẩn hóa luồng làm việc qua: Phân loại trích xuấtxuất Điều tra nguồn gốc (Root Cause Analysis) -> Đề xuất phương án xử lý (Mitigation) -> Đề xuất cải thiện hệ thống.
- **Demo thực tế:** Mô phỏng kịch bản hệ thống bị tấn công DDoS; AI tự động phân tích và đưa ra các bước khắc phục cụ thể giúp rút ngắn thời gian xử lý sự cố từ hàng giờ xuống còn vài chục phút.

#### 4. AI trong Quản trị Nhân sự (HR Modernization)
- **Thách thức của HR truyền thống:** Quy trình sàng lọc CV thủ công dễ bỏ sót ứng viên tiềm năng và thiếu một bộ khung dữ liệu chuẩn để đánh giá năng lực một cách khách quan.
- **Giải pháp Amazon Q:** Ứng dụng AI tự động đọc, phân tích và so khớp thông tin CV với mô tả công việc (JD). Hệ thống tự động phân loại mức độ phù hợp (Strong/Good/Low) và gợi ý mức lương dựa trên ngân sách hiện tại.
- **Tự động hóa luồng công việc:** Khả năng kết nối trực tiếp với hệ thống lưu trữ và giao tiếp (Gmail, Google Drive, Microsoft OneDrive) để tự động đặt lịch phỏng vấn và gửi phản hồi cho ứng viên.

#### 5. Bảo mật chuyên sâu cho AI trong doanh nghiệp (Private Security for Amazon Q)
- **Mối lo ngại về an toàn dữ liệu:** Doanh nghiệp e ngại rò rỉ các tài sản dữ liệu nội bộ quý giá ra môi trường internet công cộng khi tích hợp với AI.
- **Giải pháp kiến trúc an toàn:** Thiết lập đường truyền riêng tư tuyệt đối bằng cách kết hợp VPC Connection và MCP (Model Context Protocol) Server. Toàn bộ dữ liệu đi qua các interface endpoint, được mã hóa TLS và ẩn hoàn toàn hạ tầng khỏi môi trường internet.
- **Bài toán chi phí:** Cân đối và tối ưu các khoản phí phát sinh khi thiết lập hệ thống bảo mật chuyên sâu bao gồm Route 53 Resolver, Application Load Balancer (ALB) và chi phí truyền tải dữ liệu (Data Transfer).

### Những Gì Học Được

#### Tư Duy Thiết Kế và Phát Triển
- **Tư duy Multi-agent:** Hiểu cách phối hợp nhiều tác nhân AI chuyên biệt để giải quyết các bài toán phức tạp thay vì phụ thuộc vào một mô hình duy nhất.
- **Làm chủ nền tảng (Observability):** AI không thay thế con người, để ứng dụng AI thành thạo thì kỹ sư cốt lõi phải nắm vững các kiến thức nền tảng về hệ thống và khả năng quan sát.
- **Trải nghiệm người dùng tinh tế (UX trong AI):** Khi thiết kế các hệ thống Voice AI, cần đặc biệt lưu ý đến yếu tố con ngữ cảnh bản địa, thói quen giao tiếp và tâm lý của người dùng.

#### Kiến Trúc Kỹ Thuật và Vận Hành
- Cách xây dựng quy trình tự động hóa khắc phục sự cố Cloud và xử lý Incident tự động thông qua các đại lý AI.
- Nắm vững giải pháp thiết lập mạng lưới bảo mật thông tin nội bộ cho doanh nghiệp khi kết nối với các dịch vụ AI như Amazon Q thông qua VPC, MCP và mã hóa TLS.
- Hiểu rõ luồng kiến trúc tích hợp các công nghệ chuyển đổi ngôn ngữ (STT, TTS) kết hợp LLM để triển khai các trợ lý ảo thông minh.

#### Chiến Lược Hiện Đại Hóa Quy Trình
- Tận dụng sức mạnh của các trợ lý AI chuyên dụng (như Amazon Q) để tự động hóa các quy trình hành chính, quản trị nhân sự và sàng lọc thông tin tự động.
- Chuyển dịch từ quy trình xử lý DevOps thủ công sang mô hình tự động hóa chẩn đoán lỗi (Root Cause Analysis) bằng AI nhằm giảm thiểu tối đa "downtime" của hệ thống.

### Ứng Dụng Vào Công Việc

- **Ứng dụng AI nâng cao hiệu suất cá nhân:** Tích hợp các công cụ AI vào quy trình lập trình, tận dụng AI để tự động hóa khâu Code Review nhằm đảm bảo chất lượng source code tốt hơn.
- **Nghiên cứu kiến trúc Multi-agent:** Thử nghiệm triển khai mô hình đa tác nhân (Multi-agent) vào các dự án phần mềm cá nhân/đội nhóm để tối ưu hóa cửa sổ ngữ cảnh và phân quyền hệ thống.
- **Áp dụng giải pháp bảo mật dữ liệu:** Nghiên cứu và áp dụng các mô hình kết nối an toàn (VPC, Interface Endpoint) khi làm việc với các API của bên thứ ba nhằm bảo vệ an toàn thông tin.
- **Số hóa quy trình vận hành:** Thử nghiệm xây dựng các luồng tự động hóa đọc/trích xuất dữ liệu từ tài liệu, CV, biểu mẫu dựa trên tư duy tích hợp hệ thống của Amazon Q.

### Trải nghiệm trong event

Tham gia hội thảo **“FCAJ Community Day - June 2026”** là một trải nghiệm công nghệ vô cùng đắt giá, giúp tôi mở rộng tầm nhìn về làn sóng chuyển đổi số toàn diện dựa trên sức mạnh của Trí tuệ nhân tạo (GenAI).

#### Học hỏi từ các diễn giả có chuyên môn cao
- Tôi được lắng nghe những chia sẻ thực chiến, trực quan từ các Founder, CEO, CTO và các Kỹ sư giải pháp (Solution Specialist/Architect) hàng đầu đến từ AWS, CloudThinker, Noventiq, Renova Cloud và Cloud Kinetics.
- Những góc nhìn thực tế về sự chuyển dịch khắc nghiệt của thị trường tuyển dụng công nghệ đã mang lại cho tôi những động lực và định hướng học tập rõ ràng.

#### Trải nghiệm kỹ thuật thực tế
- Được chứng kiến các buổi Demo thực tế cực kỳ thuyết phục, đặc biệt là kịch bản đại lý AI (DevOps Agent) tự động cô lập và xử lý sự cố tấn công DDoS, tự động phân tích tìm Root Cause chỉ trong vài chục phút.
- Hiểu sâu hơn về mặt kỹ thuật hạ tầng bảo mật mạng qua sơ đồ thiết lập đường truyền mã hóa TLS ẩn toàn bộ dữ liệu doanh nghiệp khỏi internet.

#### Ứng dụng công cụ hiện đại
- Tiếp cận trực tiếp với các khái niệm và công cụ tiên phong như Nền tảng Aigentic, Amazon Q Developer, MCP Server và luồng kết hợp công nghệ xử lý giọng nói Tiếng Việt.
- Thấy rõ cách AI thâm nhập sâu và giải quyết hiệu quả các bài toán non-tech như tự động hóa quy trình tuyển dụng và so khớp năng lực nhân sự.

#### Kết nối và trao đổi
- Sự kiện tạo điều kiện kết nối tuyệt vời giữa cộng đồng kỹ sư, giúp các bạn sinh viên và lập trình viên trẻ trao đổi trực tiếp với chuyên gia để giải đáp các bài toán tối ưu chi phí vận hành (FinOps) cũng như lộ trình phát triển bản thân.

#### Bài học rút ra
- AI không sinh ra để thay thế lập trình viên, nhưng nó là một công cụ khuếch đại kỹ năng vô cùng mạnh mẽ. Người đi sau buộc phải làm chủ AI để tối ưu hóa tốc độ làm việc.
- Mọi giải pháp tích hợp AI trong doanh nghiệp đều phải đi đôi với bài toán bảo mật dữ liệu nội bộ và tối ưu chi phí hạ tầng một cách thông minh.

<!-- #### Một số hình ảnh khi tham gia sự kiện
* [Chèn hình ảnh check-in và các slide nội dung nổi bật của FCAJ Community Day tại đây] -->

> Tổng thể, sự kiện mang lại sự bứt phá lớn trong tư duy thiết kế hệ thống của tôi. Nó minh chứng rõ nét cho chủ đề của sự kiện: Khi dữ liệu được dẫn đường một cách đúng đắn, đó là lúc AI sẽ trỗi dậy mạnh mẽ để tái định hình tương lai công nghệ ("DATA DRIVEN, AI RISEN").