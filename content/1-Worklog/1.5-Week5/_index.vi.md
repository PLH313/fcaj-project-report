---
title: "Worklog Tuần 5"
date: 2026-04-06
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

* Thiết kế, xây dựng và bảo mật hệ thống quản lý tài liệu hoàn toàn không máy chủ (Serverless) trên AWS.
* Tối ưu hóa hiệu năng, bảo mật và tốc độ phân phối cho ứng dụng web.
* Triển khai thực tế các luồng xử lý dữ liệu tự động (Event-driven) cho đồ án "Hệ thống quản lý Log".

### Các công việc triển khai trong tuần này:

| STT | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Tìm hiểu: Kiến trúc Serverless, thiết kế Partition Key/Sort Key cho DynamoDB. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Khởi tạo DynamoDB lưu trữ metadata. <br> &nbsp;&nbsp;+ Lập trình Lambda thực hiện các thao tác CRUD dữ liệu. | 06/04/2026 | 06/04/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 2 | - Tìm hiểu: Luồng xác thực người dùng (Auth flow) và bảo mật dữ liệu lưu kho. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Cấu hình Cognito qua thư viện Amplify để quản lý User. <br> &nbsp;&nbsp;+ Thiết lập S3 và Bucket Policy cho upload tệp tin an toàn. | 07/04/2026 | 07/04/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 3 | - Tìm hiểu: Thiết kế RESTful API với Gateway và cấu trúc AWS SAM template. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Triển khai API Gateway kết nối Frontend và Backend. <br> &nbsp;&nbsp;+ Sử dụng AWS SAM để tự động hóa triển khai tài nguyên. | 08/04/2026 | 08/04/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 4 | - Tìm hiểu: Mã hóa dữ liệu truyền tải (In-flight) và mạng phân phối nội dung CDN. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Cấp SSL qua ACM, cấu hình Route 53 và CloudFront. <br> &nbsp;&nbsp;+ Tối ưu hóa độ trễ truy cập cho website tĩnh. | 09/04/2026 | 09/04/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 5 | - Tìm hiểu: Cơ chế đồng bộ dữ liệu qua DynamoDB Streams và lập chỉ mục tìm kiếm. <br> **- Project:** <br> &nbsp;&nbsp;+ Cài đặt CloudWatch Agent trên EC2; lập trình Lambda lọc log. <br> &nbsp;&nbsp;+ Cấu hình S3 Lifecycle Rules và đồng bộ OpenSearch cho tìm kiếm. | 10/04/2026 | 10/04/2026 | [AWS Documentation](https://docs.aws.amazon.com) |

### Kết quả đạt được tuần 5:

#### 1. Hệ thống Serverless & Web App
* Nắm vững mô hình Serverless, hiểu rõ cách phối hợp giữa Frontend, API Gateway, AWS Lambda và DynamoDB để vận hành một ứng dụng hoàn chỉnh.
* Thực hiện kiểm thử thành công các luồng API bằng Postman trước khi tích hợp vào giao diện web chính thức.

#### 2. Quản lý Hạ tầng dạng Mã (IaC)
* Trang bị kỹ năng lập trình hạ tầng chuyên nghiệp với AWS Serverless Application Model (SAM), giúp đóng gói và triển khai đồng loạt tài nguyên thay vì cấu hình thủ công.

#### 3. Bảo mật & Tối ưu hóa phân phối
* Biết cách sử dụng AWS Certificate Manager (ACM) để cấp chứng chỉ SSL/TLS, tăng cường bảo mật dữ liệu truyền tải (in-flight encryption).
* Làm chủ kỹ thuật điều hướng tên miền qua Route 53 và tối ưu hóa tốc độ tải trang bằng CDN CloudFront.

#### 4. Lõi xử lý dự án "Hệ thống quản lý Log"
* Hoàn thiện việc xây dựng lõi tiếp nhận dữ liệu tự động: Log từ EC2 được CloudWatch Agent đẩy về, kích hoạt Lambda chuẩn hóa dữ liệu và lưu trữ an toàn tại S3.
* Triển khai thành công cơ chế tối ưu chi phí dài hạn bằng cách tự động chuyển log cũ sang lớp lưu trữ S3 Glacier.

### Kiến thức tích lũy:

* **Về chuyên môn:** Nắm vững kiến trúc Event-driven và khả năng đồng bộ hóa dữ liệu thời gian thực giữa DynamoDB và OpenSearch. Hiểu sâu về quy trình bảo mật website hiện đại trên nền tảng Cloud.
* **Về kỹ năng mềm:** Phát triển tư duy hệ thống khi kết hợp nhiều dịch vụ rời rạc thành một giải pháp Serverless thống nhất. Nâng cao kỹ năng lập kế hoạch triển khai và kiểm thử ứng dụng thực tế.