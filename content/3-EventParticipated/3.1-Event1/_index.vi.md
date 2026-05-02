---
title: "Event 1"
date: 2026-03-21
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---

# Bài thu hoạch “AWS First Cloud AI Journey Community Day 2026”

### Mục Đích Của Sự Kiện

Tham gia buổi gặp gỡ cộng đồng để kết nối với các chuyên gia Cloud và lãnh đạo công nghệ, khám phá những ứng dụng mới của **Cloud & Generative AI**, cùng trải nghiệm các **demo thực tế** và mở rộng networking trong hệ sinh thái công nghệ AWS.

### Danh Sách Diễn Giả

- **Hai Bui** - Platform Engineering Manager, GoTymeX
- **Phuc (Jason) Dang** - Cloud Solution Architect, GoTymeX
- **Uyen** - Employer Branding, GoTymeX
- **Hieu Nguyen** - AI Engineer, AWS
- **Phong Nguyen** - Senior Software Engineer, AWS
- **Nguyen Hoang Viet Phap** - Cloud Engineer, VPBank
- **Phat Pham** - Software Engineer, Katalon



### Nội Dung Nổi Bật

#### 1. Building Modern Platform Engineering & GoTymeX Culture
- **Văn hóa & Cơ hội:** Giới thiệu về GoTyme – ngân hàng số đang bùng nổ tại Nam Phi, Philippines, Indonesia. Đáng chú ý, **70% nhân sự kỹ thuật** của tập đoàn đến từ Việt Nam. GoTymeX chính là trung tâm công nghệ cốt lõi với các chương trình phát triển tài năng trẻ (internship 3-6 tháng) và mô hình **mentor 1-1** bài bản.
- **Platform Engineering:** Đây là bước tiến so với Cloud Engineering truyền thống. Mục tiêu là đóng gói toàn bộ kiến thức, dịch vụ và kết nối thành sản phẩm để lập trình viên có thể tự triển khai (self-service) mà không phụ thuộc vào đội vận hành. Hệ thống tập trung vào tốc độ, độ tin cậy và sự thân thiện với developer.

#### 2. GenAIOps Essential - DevOps cho ứng dụng Generative AI
- **Sự tiến hóa kiến trúc:** Nhìn lại quá trình chuyển đổi từ **Monolithic sang Microservices** (từ năm 2012). Dù microservices giải quyết được bài toán vận hành nhưng lại tạo ra lớp phức tạp mới, đòi hỏi sự ra đời của GenAIOps.
- **Quy trình GenAIOps:** Hệ thống hóa luồng **Plan → Code → Build → Test → Release → Deploy → Operate → Monitor**.
- **Thực tiễn & Công cụ:** Sử dụng **Amazon Bedrock AgentCore** để triển khai Agent ở quy mô lớn. Ứng dụng các công cụ quan sát chuyên sâu như **Langfuse** (tracing/monitoring) và **OpenTelemetry 101** để chuẩn hóa observability trên AWS.

#### 3. Shipping Code trong kỷ nguyên AI Agent (The Agentic Era)
- **Kịch bản mới:** Thay vì quy trình cũ (một người, một tác vụ, tuần tự), kỷ nguyên Agentic cho phép nhiều Agent chạy song song.
- **Công cụ & Deep Dive:** Sử dụng **Git worktree** để cô lập môi trường cho từng Agent, tránh xung đột mã nguồn. Vai trò của lập trình viên chuyển dịch dần từ **Coder sang Supervisor** – người quản lý và điều phối các dòng chảy của Agent.
- **Năng suất vượt trội:** Các Agent có thể chia sẻ ngữ cảnh (Anthropic Agent Streams), phối hợp sửa bug và commit độc lập, giúp giải quyết tình trạng tắc nghẽn của mô hình single-agent truyền thống.

#### 4. Multimodal GenAI cấp độ Production trên AWS
- **Modern AI Stack:** Xây dựng ngăn xếp ứng dụng AI đa phương thức hoàn chỉnh, chuyển từ tìm kiếm từ khóa rời rạc sang không gian ngữ nghĩa thống nhất.
- **Công nghệ tiên phong:** 
    - **Nova Embeddings:** Đồng nhất văn bản, hình ảnh, video, âm thanh vào cùng một không gian vector với độ chính xác cao.
    - **GraphRAG:** Kết hợp cơ sở dữ liệu đồ thị với RAG để khai thác tri thức doanh nghiệp sâu sắc hơn.
- **An toàn & Giám sát:** Triển khai serverless mở rộng dễ dàng, kết hợp với **Bedrock Guardrails** để đảm bảo tính tuân thủ và an toàn tuyệt đối cho dữ liệu.

#### 5. Cảm hứng từ cộng đồng FCAJ
- **Vượt qua giới hạn:** Câu chuyện về những thành viên khiếm thính trong cộng đồng FCAJ vẫn miệt mài sáng tạo và làm chủ công nghệ Cloud.
- **Tinh thần đồng đội:** Họ không chỉ học cho mình mà còn chủ động hỗ trợ, hướng dẫn các bạn khiếm thính mới gia nhập hòa nhập với hệ sinh thái công nghệ. Đây là minh chứng rõ nhất cho việc đam mê có thể vượt qua mọi rào cản vật lý.



### Những Gì Học Được

#### Tư Duy Thiết Kế & Vận Hành
- **Platform Thinking:** Hiểu rằng Platform Engineering là tạo ra "đường băng" để lập trình viên tập trung vào Business Logic mà không bị gánh nặng hạ tầng làm chậm nhịp độ.
- **GenAIOps Mindset:** Quản lý ứng dụng AI là một vòng lặp liên tục, cần sự phối hợp chặt chẽ giữa CI/CD, tự động hóa IaC và văn hóa hợp tác giữa các nhóm.

#### Kiến Trúc Kỹ Thuật
- **Kiến trúc Multi-Agent:** Cách vận hành nhiều Agent song song và sử dụng Git worktree để tối ưu hóa hiệu suất lập trình.
- **Multimodal AI:** Sức mạnh của việc thống nhất các loại dữ liệu (văn bản, video, âm thanh) để tạo ra các giải pháp tìm kiếm doanh nghiệp thông minh (GraphRAG).

#### Chiến Lược Hiện Đại Hóa
- **Agentic Workflow:** Tầm quan trọng của Prompt/Context engineering trong việc điều phối các Agent.
- **Observability:** Tầm quan trọng của việc giám sát và tracing (Langfuse) để đảm bảo hệ thống AI hoạt động ổn định trong thực tế.



### Ứng Dụng Vào Công Việc

- **Áp dụng nguyên tắc Platform Engineering:** Xây dựng các hệ thống có tính tái sử dụng cao, hỗ trợ developer tự chủ trong việc triển khai tài nguyên.
- **Triển khai Pipeline GenAIOps:** Thiết lập quy trình CI/CD tự động cho các ứng dụng AI sinh tạo tại công ty, tích hợp khả năng quan sát (observability).
- **Thử nghiệm quy trình đa Agent:** Sử dụng Git worktrees và agent supervisors để tăng năng suất refactor code và phát triển tính năng mới.
- **Thí điểm giải pháp AI đa phương thức:** Áp dụng Nova embeddings và GraphRAG vào việc quản lý và truy xuất kho tri thức nội bộ của doanh nghiệp.
- **Thúc đẩy văn hóa hòa nhập:** Lấy cảm hứng từ FCAJ để xây dựng môi trường làm việc đa dạng, hỗ trợ mọi thành viên cùng phát triển.



### Trải nghiệm trong event

Tham dự sự kiện là một hành trình khám phá đầy cảm hứng, giúp em thay đổi hoàn toàn tư duy về thiết kế ứng dụng và phối hợp nhóm.

#### Học hỏi từ các diễn giả tiên phong
- Được lắng nghe các **best practices** về platform engineering và GenAIOps từ những kỹ sư hàng đầu tại GoTymeX và AWS.
- Các case study thực tế giúp em nhận ra những thách thức thật sự khi vận hành microservices ở quy mô lớn.

#### Trải nghiệm kỹ thuật thực tế
- Các phiên demo trực tiếp về **AI Agent** và **GraphRAG** mang lại cái nhìn trực quan, giúp những khái niệm phức tạp trở nên dễ hiểu hơn bao giờ hết.
- Hiểu rõ cách **Amazon Bedrock** hỗ trợ triển khai agent quy mô lớn và cách các framework giám sát (Langfuse) bảo vệ hệ thống.

#### Bài học rút ra
- AI không thay thế lập trình viên, nhưng lập trình viên biết cách giám sát và điều phối Agent sẽ tạo ra giá trị đột phá.
- Công nghệ luôn chuyển dịch rất nhanh, việc duy trì tinh thần học hỏi liên tục và xây dựng cộng đồng hỗ trợ nhau (như FCAJ) là yếu tố sống còn trong ngành Cloud.

#### Một số hình ảnh khi tham gia sự kiện
![GoTymeX 1](/images/3-EventParticipated/3.1-Event1/event_img1.jpg)
![GoTymeX 2](/images/3-EventParticipated/3.1-Event1/event_img2.jpg)
![GenAIOps Essential](/images/3-EventParticipated/3.1-Event1/event_img3.jpg)
![Shipping Code Agentic Era](/images/3-EventParticipated/3.1-Event1/event_img4.jpg)
![Multimodal GenAI](/images/3-EventParticipated/3.1-Event1/event_img5.jpg)

> Tổng kết, sự kiện "AWS First Cloud AI Journey Community Day 2026" không chỉ cập nhật kiến thức kỹ thuật mà còn là bệ phóng giúp em định hình rõ ràng con đường hiện đại hóa hạ tầng và ứng dụng AI vào thực tế sản xuất. 