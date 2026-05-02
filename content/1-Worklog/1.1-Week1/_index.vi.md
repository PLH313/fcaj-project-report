---
title: "Worklog Tuần 1"
date: 2026-03-09
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Mục tiêu tuần 1:

* Nghiên cứu tài liệu kiến thức nền tảng về kiến trúc các dịch vụ AWS cốt lõi.
* Trực tiếp thực hiện chuỗi bài Lab thực hành để nắm bắt luồng vận hành thực tế của hệ thống.
* Thiết lập môi trường quản trị an toàn và tối ưu chi phí ngay từ giai đoạn đầu.

### Các công việc triển khai trong tuần này:

| STT | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Tìm hiểu: Bảo mật tài khoản Root, sự khác biệt giữa Root User và IAM User. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Khởi tạo tài khoản, thiết lập Virtual MFA cho Root. <br> &nbsp;&nbsp;+ Tạo IAM Admin Group/User. <br> &nbsp;&nbsp;+ Tùy chỉnh Console (Region, Dashboard Widgets). | 09/03/2026 | 09/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 2 | - Tìm hiểu: Cơ chế tính phí (Free Tier, Pay-as-you-go) và các gói AWS Support. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Thiết lập 4 loại AWS Budget (Cost, Usage, RI, Savings Plans). <br> &nbsp;&nbsp;+ Thực hành quy trình tạo Support Case. | 10/03/2026 | 10/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 3 | - Tìm hiểu: Phân quyền nâng cao với IAM Role, giao diện dòng lệnh AWS CLI. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Tạo Role cho Admin/Operator và thực hành Switch Role. <br> &nbsp;&nbsp;+ Khởi tạo Cloud9 IDE và thao tác qua CLI. | 11/03/2026 | 11/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 4 | - Tìm hiểu: Thành phần kiến trúc Amazon VPC (Subnets, IGW, NAT Gateway, Route Table). <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Thiết kế VPC: Cấu hình Public/Private Subnets. <br> &nbsp;&nbsp;+ Thiết lập lá chắn bảo mật Security Group. <br> &nbsp;&nbsp;+ Giả lập kết nối Site-to-Site VPN an toàn. | 12/03/2026 | 13/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 5 | - Tìm hiểu: Dịch vụ EC2 (Instance Types, AMI, EBS) và Best Practice bảo mật. <br> **- Thực hành Project (Log Management):** <br> &nbsp;&nbsp;+ Triển khai máy chủ EC2 Linux & Windows. <br> &nbsp;&nbsp;+ Cài đặt LAMP stack và ứng dụng Node.js. <br> &nbsp;&nbsp;+ Gắn IAM Role cho EC2 để truy cập S3 tự động. | 13/03/2026 | 13/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |



### Kết quả đạt được tuần 1:

#### 1. Quản trị Tài khoản & Bảo mật
* Hoàn tất bảo mật tài khoản Root bằng MFA. Triển khai mô hình quản trị an toàn qua Admin User và Admin Group.
* Phân tích và nắm rõ sự khác biệt giữa các gói AWS Support (Basic, Developer, Business, Enterprise) và quy trình xử lý sự cố qua Support Case.
* Thực hiện thành thạo cơ chế **Switch Role** để quản lý quyền truy cập chéo giữa các tài khoản mà không cần chia sẻ thông tin đăng nhập.

#### 2. Kiểm soát Chi phí
* Thiết lập thành công hệ thống cảnh báo ngân sách tự động cho 4 danh mục cốt lõi: Chi phí, Mức sử dụng, Reserved Instances (RI) và Savings Plans.
* Cấu hình ngưỡng cảnh báo tại 80% và 100% giúp chủ động kiểm soát tài nguyên.

#### 3. Hạ tầng Mạng & Kết nối
* Xây dựng thành công môi trường mạng biệt lập (VPC) với đầy đủ các thành phần điều hướng (Route Table) và lá chắn bảo mật (Security Group).
* Triển khai hệ thống cho phép máy chủ nội bộ (Private Subnet) truy cập internet an toàn qua NAT Gateway và giả lập kết nối VPN an toàn giữa On-premise và AWS.

#### 4. Máy chủ ảo & Ứng dụng
* Triển khai và quản trị máy chủ EC2 trên cả nền tảng Linux và Windows. Làm chủ các tác vụ: tạo Snapshot, đóng gói Custom AMI và viết Policy giới hạn Instance Type/Region.
* Áp dụng **Best Practice** về bảo mật: Sử dụng IAM Role gắn trực tiếp vào EC2 instance để ứng dụng truy cập S3 tự động, loại bỏ hoàn toàn rủi ro lộ Access Key/Secret Key trong mã nguồn.
* Làm quen và thao tác thành thạo trên môi trường phát triển **AWS Cloud9**, sử dụng giao diện dòng lệnh (CLI) để truy vấn và quản lý tài nguyên.



### Kiến thức tích lũy:

* **Về chuyên môn:** Hiểu rõ cơ chế vận hành từ hạ tầng vật lý ảo hóa (EC2, VPC) đến các lớp bảo mật logic (IAM, Security Group). Củng cố tư duy thiết kế hệ thống an toàn và tối ưu chi phí trên nền tảng Cloud thông qua các kịch bản phân quyền phức tạp.
* **Về kỹ năng mềm:** Rèn luyện khả năng đọc hiểu tài liệu chuyên ngành (AWS Documentation), nâng cao kỹ năng xử lý sự cố (troubleshooting) khi cấu hình hạ tầng mạng và hình thành tác phong làm việc, báo cáo độc lập chuyên nghiệp.