---
title: "Worklog Tuần 2"
date: 2026-03-16
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

* Đi sâu vào việc triển khai, giám sát và tự động hóa hệ thống trên nền tảng AWS.
* Thực hành mở rộng quy mô kiến trúc (Scaling) và quản lý đa dạng các loại cơ sở dữ liệu (SQL & NoSQL).
* Làm quen với container hóa ứng dụng và cấu hình các giải pháp mạng nâng cao.

### Các công việc triển khai trong tuần này:

| STT | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Tìm hiểu: Các loại lưu trữ S3 (Storage Classes) và nguyên lý Static Website Hosting. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Khởi tạo bucket và cấu hình Static Website. <br> &nbsp;&nbsp;+ Thực hành di chuyển và điều phối dữ liệu giữa các buckets. | 16/03/2026 | 16/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 2 | - Tìm hiểu: Sự khác biệt giữa SQL (RDS) và NoSQL (DynamoDB); cơ chế phân quyền bảo mật DB. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Thiết lập hạ tầng mạng cho RDS; cấu hình EC2 kết nối RDS. <br> &nbsp;&nbsp;+ Thao tác ghi và truy vấn dữ liệu NoSQL qua bảng DynamoDB. | 17/03/2026 | 17/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 3 | - Tìm hiểu: Kiến trúc Docker, Container Registry và ưu điểm của Lightsail cho dự án nhỏ. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Cài đặt Docker, build/push image lên registry. <br> &nbsp;&nbsp;+ Triển khai Container Service và thiết lập cảnh báo tài nguyên. | 17/03/2026 | 18/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 4 | - Tìm hiểu: Nguyên lý cân bằng tải (Load Balancing) và tự động giãn nở (Auto Scaling). <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Cấu hình ALB và ASG để đảm bảo tính sẵn sàng cao. <br> &nbsp;&nbsp;+ Thiết lập CloudWatch Logs/Metrics và Alarms qua SNS. | 18/03/2026 | 19/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 5 | - Tìm hiểu: Tư duy Infrastructure as Code (IaC) và giải pháp Hybrid DNS. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Sử dụng CloudFormation template để khởi tạo hạ tầng. <br> &nbsp;&nbsp;+ Cấu hình Route 53 Outbound Endpoints kết nối On-premises. | 19/03/2026 | 20/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |

### Kết quả đạt được tuần 2:

#### 1. Lưu trữ & Cơ sở dữ liệu
* Làm chủ kỹ thuật triển khai website tĩnh trên S3 và các thao tác điều hướng dữ liệu hiệu quả.
* Hiểu rõ phương thức khởi tạo, bảo mật cơ sở dữ liệu quan hệ (RDS) và thực hiện truy vấn hiệu năng cao trên cơ sở dữ liệu phi quan hệ (DynamoDB).

#### 2. Tính sẵn sàng cao & Giám sát
* Nắm vững nguyên lý thiết kế Fault Tolerance thông qua việc phối hợp ALB và ASG để tự động điều chỉnh quy mô tài nguyên theo nhu cầu người dùng.
* Triển khai hệ thống giám sát tập trung với CloudWatch, cho phép tự động gửi thông báo cảnh báo khi phát hiện sự cố hệ thống hoặc tài nguyên vượt ngưỡng.

#### 3. Container hóa & Tự động hóa
* Thực hành thành thạo quy trình build image với Docker và quản lý container thông qua Lightsail Container Service.
* Làm quen với tư duy quản lý hạ tầng dưới dạng mã (IaC) bằng CloudFormation giúp nhanh chóng khởi tạo các môi trường mạng phức tạp.

#### 4. Quản trị hệ thống nâng cao
* Nâng cao tốc độ quản trị tài nguyên S3 thông qua giao diện dòng lệnh AWS CLI.
* Hiểu và cấu hình thành công giải pháp Hybrid DNS để xử lý truy vấn giữa môi trường on-premises và đám mây.

### Kiến thức tích lũy:

* **Về chuyên môn:** Hiểu rõ cách lựa chọn loại cơ sở dữ liệu phù hợp với bài toán. Hình thành tư duy vận hành (Ops) chuyên nghiệp thông qua việc kết hợp giám sát và container hóa.
* **Về kỹ năng mềm:** Phát triển tư duy tự động hóa, nâng cao khả năng xử lý lỗi độc lập và kỹ năng áp dụng tài liệu kỹ thuật vào các mô hình kiến trúc thực tế.