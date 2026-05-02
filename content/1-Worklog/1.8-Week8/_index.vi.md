---
title: "Worklog Tuần 8"
date: 2026-04-27
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

* Hoàn thiện kiến trúc bảo mật và xác thực người dùng cho toàn bộ hệ thống đồ án.
* Triển khai giải pháp quản lý định danh và bảo mật cổng giao tiếp ứng dụng.
* Chạy kiểm thử toàn diện hệ thống (End-to-End) và đóng gói hồ sơ báo cáo tổng kết thực tập.

### Các công việc triển khai trong tuần này:

| STT | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Tìm hiểu: Các mô hình Authentication và Authorization cho hệ thống Dashboard quản lý. <br> **- Project:** <br> &nbsp;&nbsp;+ Phân tích và lên phương án xác thực người dùng cho Dashboard quản trị Log. | 27/04/2026 | 27/04/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 2 | - Tìm hiểu: Cơ chế bảo mật cổng giao tiếp (API Security) và quản lý danh tính tập trung. <br> **- Project:** <br> &nbsp;&nbsp;+ Triển khai Amazon Cognito để quản lý định danh người dùng. | 28/04/2026 | 28/04/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 3 | - Tìm hiểu: Lợi ích của AWS App Runner trong việc vận hành Web App mà không cần quản lý máy chủ. <br> **- Project:** <br> &nbsp;&nbsp;+ Triển khai ứng dụng quản lý ổn định trên nền tảng AWS App Runner. | 29/04/2026 | 29/04/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 4 | **- Project:** <br> &nbsp;&nbsp;+ Chạy kiểm thử End-to-End toàn diện từ EC2 đến Dashboard. <br> &nbsp;&nbsp;+ Khắc phục lỗi đồng bộ phân vùng Athena và tinh chỉnh quyền hạn IAM cuối cùng. | 30/04/2026 | 01/05/2026 | |
| 5 | **- Project:** <br> &nbsp;&nbsp;+ Tổng hợp tài liệu kỹ thuật và vẽ lưu đồ dữ liệu cuối cùng. <br> &nbsp;&nbsp;+ Hoàn thiện báo cáo thực tập. | 01/05/2026 | 01/05/2026 | |

### Kết quả đạt được tuần 8:

#### 1. Bảo mật & Xác thực người dùng
* Triển khai thành công hệ thống quản lý danh tính với Amazon Cognito, cho phép người dùng đăng nhập vào Dashboard quản trị log một cách an toàn.
* Nắm vững cách thiết lập bảo mật cổng giao tiếp ứng dụng, đảm bảo dữ liệu log chỉ được truy cập bởi những đối tượng đã được định danh.

#### 2. Vận hành ứng dụng hiện đại
* Làm chủ quy trình triển khai ứng dụng nhanh chóng qua AWS App Runner, giúp tự động hóa khâu hạ tầng cho các ứng dụng web và API mà không cần quản lý máy chủ.

#### 3. Hoàn thiện luồng dữ liệu End-to-End
* Hệ thống đã vượt qua các bài kiểm thử chịu tải và kiểm thử logic: Log từ EC2 -> SQS -> Lambda -> S3 & DynamoDB -> API Gateway -> Dashboard hiển thị mượt mà.
* Khắc phục hoàn toàn các lỗi tồn đọng về đồng bộ phân vùng trên Athena và các vấn đề về quyền hạn IAM cuối cùng.

#### 4. Tổng kết thực tập
* Hoàn thành bộ hồ sơ báo cáo thực tập chuyên sâu, phản ánh đầy đủ quá trình từ việc làm quen dịch vụ cơ bản đến việc xây dựng kiến trúc Serverless Event-driven phức tạp.

### Kiến thức tích lũy:

* **Về chuyên môn:** Hiểu rõ cách tích hợp lớp bảo mật Authentication vào hệ thống Cloud thực tế. Có cái nhìn tổng quan về quy trình phát triển dự án từ khâu thiết kế kiến trúc đến khâu đóng gói sản phẩm.
* **Về kỹ năng mềm:** Rèn luyện kỹ năng tổng hợp thông tin và viết báo cáo kỹ thuật. Củng cố khả năng làm việc độc lập và quản lý thời gian để hoàn thành mục tiêu dự án đúng thời hạn.