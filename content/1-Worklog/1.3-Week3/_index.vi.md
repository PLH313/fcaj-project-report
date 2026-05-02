---
title: "Worklog Tuần 3"
date: 2026-03-23
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:

* Tập trung tối ưu hóa hiệu năng ứng dụng thông qua các giải pháp bộ nhớ đệm và phân phối nội dung.
* Mở rộng hạ tầng mạng nâng cao và triển khai các giải pháp quản trị hệ thống tập trung.
* Tìm hiểu các tính năng nâng cao của hạ tầng dưới dạng mã (IaC) để chuẩn bị cho dự án nhóm.

### Các công việc triển khai trong tuần này:

| STT | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Tìm hiểu: Cơ chế lưu trữ In-memory, so sánh Redis và Memcached. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Khởi tạo Amazon ElastiCache (Redis Cluster). <br> &nbsp;&nbsp;+ Sử dụng AWS SDK để thực hiện các lệnh đọc/ghi dữ liệu hiệu năng cao. | 23/03/2026 | 23/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 2 | - Tìm hiểu: Kiến trúc Hub-and-spoke với Transit Gateway và các mô hình kết nối mạng liên vùng. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Thiết lập VPC Peering và Transit Gateway. <br> &nbsp;&nbsp;+ Cấu hình kết nối Site-to-Site VPN. | 24/03/2026 | 24/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 3 | - Tìm hiểu: Route 53 Resolver cho mạng Hybrid và nguyên lý mạng phân phối nội dung (CDN). <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Cấu hình CloudFront Distribution với Cache Behavior. <br> &nbsp;&nbsp;+ Triển khai Lambda@Edge tại các điểm biên toàn cầu. | 25/03/2026 | 25/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 4 | - Tìm hiểu: Phương pháp quản trị máy chủ quy mô lớn không cần mở cổng 22/3389. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Sử dụng Systems Manager (SSM) Run Command thực thi lệnh hàng loạt. <br> &nbsp;&nbsp;+ Kết nối máy chủ an toàn qua Session Manager. | 26/03/2026 | 26/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 5 | - Tìm hiểu: CloudFormation Custom Resources sử dụng Lambda trigger. <br> **- Project:** <br> &nbsp;&nbsp;+ Họp nhóm thống nhất kiến trúc phân tách RDS/DynamoDB cho đồ án. <br> &nbsp;&nbsp;+ Chốt sơ đồ luồng dữ liệu Frontend (S3/CloudFront) và Backend. | 27/03/2026 | 27/03/2026 | [AWS Documentation](https://docs.aws.amazon.com) |

### Kết quả đạt được tuần 3:

#### 1. Tối ưu hóa Hiệu năng & Phân phối
* Hiểu và triển khai thành công cơ chế lưu trữ dữ liệu trong bộ nhớ với ElastiCache - Redis giúp giảm tải đáng kể cho cơ sở dữ liệu chính.
* Làm chủ kỹ thuật cấu hình CloudFront Distribution và Lambda@Edge để tối ưu hóa trải nghiệm người dùng tại các vị trí địa lý khác nhau.

#### 2. Hạ tầng Mạng Hybrid & Bảo mật
* Nắm vững kỹ năng thiết kế mạng Hybrid thông qua việc kết hợp Transit Gateway và VPN để bảo mật đường truyền giữa hạ tầng on-premises và đám mây.
* Nghiên cứu thành công cơ chế chuyển tiếp truy vấn DNS thông qua Route 53 Resolver.

#### 3. Quản trị máy chủ tập trung
* Sử dụng thành thạo AWS Systems Manager để quản lý bản vá và thực thi lệnh hàng loạt trên các máy chủ Windows EC2.
* Loại bỏ hoàn toàn nhu cầu sử dụng Bastion Host nhờ triển khai Session Manager, giúp giảm thiểu rủi ro bảo mật từ việc mở các cổng quản trị trực tiếp (22/3389).

#### 4. Hạ tầng dạng mã & Định hình dự án
* Tiếp cận các tính năng nâng cao của CloudFormation, đặc biệt là việc sử dụng Lambda làm Custom Resources để khởi tạo các tài nguyên phức tạp.
* Thống nhất kiến trúc dự án: Sử dụng S3/CloudFront cho Frontend, Lambda/EC2 cho xử lý trung tâm và kết hợp RDS với DynamoDB để tối ưu lưu trữ dữ liệu.

### Kiến thức tích lũy:

* **Về chuyên môn:** Hiểu rõ phương thức tối ưu hóa hệ thống qua bộ nhớ đệm và mạng phân phối nội dung toàn cầu. Hình thành tư duy quản trị máy chủ hiện đại không cần Bastion Host.
* **Về kỹ năng mềm:** Phát triển tư duy tự động hóa hạ tầng chuyên nghiệp. Nâng cao khả năng phối hợp nhóm và kỹ năng lập kế hoạch kiến trúc hệ thống cho các dự án thực tế.