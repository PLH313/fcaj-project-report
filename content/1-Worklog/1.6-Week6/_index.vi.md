---
title: "Worklog Tuần 6"
date: 2026-04-13
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

* Tập trung nghiên cứu và thực hành các giải pháp bảo mật và quản lý định danh chuyên sâu trên AWS.
* Tiếp tục phát triển và tối ưu hóa các module xử lý dữ liệu cho đồ án "Hệ thống quản lý Log".
* Thực hiện kiểm thử tích hợp nội bộ để đảm bảo tính ổn định của luồng dữ liệu cốt lõi.

### Các công việc triển khai trong tuần này:

| STT | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Tìm hiểu: Cơ chế Single Sign-On (SSO) và quản trị đa tài khoản với AWS Organizations. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Thiết lập AWS IAM Identity Center (SSO) để quản lý truy cập tập trung. | 13/04/2026 | 13/04/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 2 | - Tìm hiểu: Rủi ro leo thang đặc quyền và các biến điều kiện (Condition Keys) trong IAM Policy. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Cấu hình IAM Permission Boundary để giới hạn quyền tối đa cho User. <br> &nbsp;&nbsp;+ Thiết lập IAM Role với các điều kiện chặt chẽ về IP và thời gian truy cập. | 14/04/2026 | 14/04/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 3 | - Tìm hiểu: Tiêu chuẩn bảo mật CIS và cơ chế ghi lại lịch sử thay đổi tài nguyên. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Kích hoạt AWS Config; thiết lập Security Hub để chấm điểm tuân thủ bảo mật. | 15/04/2026 | 15/04/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 4 | - Tìm hiểu: Các kiểu tấn công Web phổ biến (SQL Injection, XSS) và phân tích hành vi bất thường. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Cấu hình GuardDuty giám sát đe dọa; triển khai AWS WAF bảo vệ ứng dụng. | 16/04/2026 | 16/04/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 5 | - Tìm hiểu: Quản lý khóa đối xứng KMS và cấu trúc log truy vết CloudTrail. <br> **- Project:** <br> &nbsp;&nbsp;+ Sử dụng KMS mã hóa dữ liệu; truy vấn log CloudTrail bằng Athena. <br> &nbsp;&nbsp;+ Tối ưu code Lambda parsing JSON và kiểm thử tích hợp luồng dữ liệu đến S3. | 17/04/2026 | 17/04/2026 | [AWS Documentation](https://docs.aws.amazon.com) |

### Kết quả đạt được tuần 6:

#### 1. Bảo mật hạ tầng & Quản lý định danh
* Hiểu rõ bức tranh tổng thể về bảo mật trên AWS thông qua việc phối hợp giữa IAM Identity Center, AWS Config, CloudTrail và AWS WAF.
* Nắm vững kỹ thuật thiết lập "hàng rào bảo vệ" bằng Permission Boundary, giúp ngăn chặn rủi ro leo thang đặc quyền trong hệ thống.

#### 2. Giám sát & Phát hiện mối đe dọa
* Triển khai thành công hệ thống phát hiện hành vi xâm nhập trái phép với Amazon GuardDuty dựa trên phân tích VPC Flow Logs và DNS Logs.
* Biết cách sử dụng Security Hub để theo dõi mức độ tuân thủ bảo mật của tài khoản so với các tiêu chuẩn quốc tế.

#### 3. Mã hóa & Phân tích dữ liệu truy vết
* Làm chủ quy trình mã hóa dữ liệu bằng khóa đối xứng trong KMS và cách truy vết mọi thao tác trên hệ thống thông qua CloudTrail.
* Sử dụng thành thạo Amazon Athena để thực hiện các truy vấn SQL phức tạp trực tiếp trên dữ liệu log thô, phục vụ mục đích kiểm tra và báo cáo.

#### 4. Tiến độ Đồ án "Hệ thống quản lý Log"
* Tối ưu hóa thành công hiệu suất của hàm Lambda, giúp xử lý các dòng log định dạng JSON nhanh chóng và chính xác hơn.
* Đảm bảo luồng dữ liệu từ lúc CloudWatch Agent thu thập, Lambda xử lý lọc log lỗi (Error/Warning) và lưu trữ vào Amazon S3 hoạt động ổn định qua các bài test tích hợp.

### Kiến thức tích lũy:

* **Về chuyên môn:** Nắm vững cách phối hợp các dịch vụ bảo mật AWS để tạo ra một hệ thống phòng thủ đa lớp. Thành thạo việc sử dụng môi trường dòng lệnh (WSL) để cấu hình các chính sách IAM phức tạp mà giao diện Console khó đáp ứng nhanh.
* **Về kỹ năng mềm:** Nâng cao tư duy "Security by Design" (Bảo mật ngay từ khâu thiết kế). Rèn luyện kỹ năng troubleshooting khi xử lý các lỗi phân quyền và tối ưu hóa mã nguồn trong môi trường thực tế.