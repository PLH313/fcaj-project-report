---
title: "Worklog Tuần 7"
date: 2026-04-20
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Tái cấu trúc toàn bộ đồ án sang kiến trúc Serverless nâng cao để giải quyết vấn đề nghẽn cổ chai (bottleneck).
* Triển khai cơ chế hàng đợi (Message Queue) để điều phối luồng dữ liệu log ổn định.
* Tối ưu hóa cấu trúc lưu trữ và truy vấn dữ liệu lớn trên S3 bằng Hive Partitioning và Amazon Athena.

### Các công việc triển khai trong tuần này:

| STT | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Tìm hiểu: Kiến trúc luồng Data Routing và ưu điểm của SQS FIFO trong việc đảm bảo thứ tự dữ liệu. <br> **- Project:** <br> &nbsp;&nbsp;+ Chuyển đổi luồng dữ liệu sang sử dụng SQS FIFO làm bộ đệm xử lý trung tâm. | 20/04/2026 | 20/04/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 2 | - Tìm hiểu: Logic Alert Debounce và cách kiểm soát trạng thái cảnh báo dựa trên timestamp. <br> **- Project:** <br> &nbsp;&nbsp;+ Xây dựng thuật toán chặn cảnh báo lặp lại từ SNS dựa trên trạng thái thời gian truy vấn từ DynamoDB. | 21/04/2026 | 21/04/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 3 | - Tìm hiểu: Cơ chế Hive Partitioning và các câu lệnh DDL nâng cao trong Amazon Athena. <br> **- Project:** <br> &nbsp;&nbsp;+ Nâng cấp lưu trữ S3: Triển khai cấu trúc phân vùng (year/month/day/appid). <br> &nbsp;&nbsp;+ Đồng bộ hóa phân vùng dữ liệu bằng Athena. | 22/04/2026 | 22/04/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 4 | - Tìm hiểu: Tích hợp Lambda với HTTP API Gateway và cơ chế xác thực cho Client Dashboard. <br> **- Project:** <br> &nbsp;&nbsp;+ Rà soát luồng tích hợp giữa API Gateway và Lambda xử lý truy xuất dữ liệu. | 23/04/2026 | 23/04/2026 | [AWS Documentation](https://docs.aws.amazon.com) |
| 5 | - Tìm hiểu: Cơ chế Time to Live (TTL) của DynamoDB và S3 Lifecycle Management. <br> **- Project:** <br> &nbsp;&nbsp;+ Cấu hình S3 Lifecycle Rule; tạo bảng DynamoDB với cơ chế TTL. <br> &nbsp;&nbsp;+ Đóng gói mã nguồn Python và thiết lập SQS làm Event Trigger cho Lambda. | 24/04/2026 | 24/04/2026 | [AWS Documentation](https://docs.aws.amazon.com) |

### Kết quả đạt được tuần 7:

#### 1. Kiến trúc hệ thống nâng cao
* Chuyển đổi thành công từ mô hình thu thập log truyền thống sang kiến trúc Serverless phân tán, sử dụng hàng đợi SQS FIFO để đảm bảo thứ tự và khả năng chịu tải của hệ thống.
* Nắm vững cách bóc tách JSON từ Lambda Consumer để phân phối đồng thời dữ liệu vào kho lạnh (S3) và kho nóng (DynamoDB).

#### 2. Tối ưu hóa cảnh báo
* Giải quyết triệt để tình trạng "dội bom" email bằng thuật toán Alert Debounce, cho phép kiểm soát tần suất cảnh báo của SNS trong khung thời gian 15 phút.

#### 3. Quản trị dữ liệu quy mô lớn
* Định hình được cấu trúc Hive Partitioning trên S3, giúp tối ưu hóa không gian lưu trữ và tăng tốc độ truy vấn đáng kể cho Amazon Athena.
* Thiết lập thành công cơ chế TTL (Time to Live) trên DynamoDB để tự động dọn dẹp các log trạng thái, giúp duy trì hiệu năng bảng và tiết kiệm chi phí.

#### 4. Triển khai và Tích hợp hạ tầng
* Triển khai và kết nối luồng sự kiện giữa các dịch vụ cốt lõi (SQS, Lambda, S3, DynamoDB, SNS) thông qua việc cấu hình các chính sách IAM Role chặt chẽ và an toàn.

### Kiến thức tích lũy:

* **Về chuyên môn:** Hiểu sâu sắc sự khác biệt giữa kiến trúc đồng bộ và bất đồng bộ trong việc xử lý log. Nắm vững kỹ thuật phân vùng dữ liệu Hive để xử lý Big Data trên nền tảng Cloud.
* **Về kỹ năng mềm:** Phát triển khả năng phân tích mã nguồn Python chuyên sâu. Rèn luyện tư duy tối ưu hóa kiến trúc (Optimization) để đáp ứng các bài toán thực tế về hiệu năng và chi phí.