---
title: "Worklog Tuần 4"
date: 2026-03-30
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* Tập trung vào các giải pháp giám sát và tối ưu hóa chi phí hệ thống máy chủ.
* Thực hành đóng gói và triển khai ứng dụng thông qua công nghệ Container.
* Thống nhất đề tài và xây dựng kiến trúc cốt lõi cho dự án "Hệ thống quản lý Log".

### Các công việc triển khai trong tuần này:

| STT | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :---: | :---: | :--- |
| 1 | - Tìm hiểu: Cơ chế Event-driven và lập lịch tác vụ với AWS Lambda. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Lập trình Lambda tự động bật/tắt EC2 theo khung giờ thực tế để tối ưu chi phí. | 30/03/2026 | 30/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 2 | - Tìm hiểu: Kiến trúc Docker, quy trình quản lý vòng đời Image và Amazon ECR. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Đóng gói ứng dụng Web Server và Database bằng Docker. <br> &nbsp;&nbsp;+ Quản lý và lưu trữ hình ảnh ứng dụng trên Amazon ECR. | 31/03/2026 | 31/03/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 3 | - Tìm hiểu: Các chỉ số giám sát hệ thống (Metrics) và cơ chế Log tập trung. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Cấu hình CloudWatch Metrics, Logs và thiết lập Alarm. <br> &nbsp;&nbsp;+ Xây dựng Dashboard giám sát trực quan cho tài nguyên. | 01/04/2026 | 01/04/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 4 | - Tìm hiểu: Khái niệm "Right-sizing" và cách đọc đề xuất từ AWS Compute Optimizer. <br> **- Thực hành:** <br> &nbsp;&nbsp;+ Cài đặt CloudWatch Agent phối hợp với Compute Optimizer để chọn cấu hình EC2. <br> &nbsp;&nbsp;+ Bật VPC Flow Logs để giám sát lưu lượng mạng IP. | 02/04/2026 | 03/04/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com) |
| 5 | - Tìm hiểu: Kiến trúc hệ thống quản lý log quy mô lớn trên Cloud. <br> **-  Project:** <br> &nbsp;&nbsp;+ Thống nhất xây dựng dự án dựa trên bộ ba: CloudWatch, Lambda và S3. <br> &nbsp;&nbsp;+ Thiết kế sơ đồ luồng dữ liệu log từ thu thập đến lưu trữ lâu dài. | 03/04/2026 | 03/04/2026 | [AWS Documentation](https://docs.aws.amazon.com) |

### Kết quả đạt được tuần 4:

#### 1. Công nghệ Container & Quản lý Image
* Nắm vững kiến thức cốt lõi về việc container hóa ứng dụng bằng Docker.
* Thành thạo quy trình quản lý kho lưu trữ image trên đám mây thông qua Amazon Elastic Container Registry (ECR).

#### 2. Giám sát & Đo lường hệ thống
* Hiểu và biết cách triển khai các công cụ giám sát từ cơ bản đến nâng cao với Amazon CloudWatch.
* Có khả năng phân tích chi tiết lưu lượng mạng đi vào và đi ra khỏi VPC thông qua VPC Flow Logs để phát hiện các bất thường về hạ tầng.

#### 3. Tối ưu hóa tài nguyên & Chi phí
* Hình thành tư duy tối ưu hóa (Cost Optimization) thông qua việc tự động hóa các tác vụ vận hành bằng AWS Lambda.
* Biết cách sử dụng số liệu thực tế từ CloudWatch Agent để thực hiện "Right-sizing", giúp lựa chọn cấu hình máy chủ hiệu quả nhất về mặt chi phí và hiệu năng.

#### 4. Định hình kiến trúc dự án
* Xác lập được luồng dữ liệu cốt lõi cho dự án cuối kỳ: Sử dụng CloudWatch để thu thập tập trung, Lambda xử lý sự kiện và S3 làm kho lưu trữ lâu dài.

### Kiến thức tích lũy:

* **Về chuyên môn:** Hiểu rõ tầm quan trọng của việc giám sát liên tục và tối ưu hóa tài nguyên dựa trên dữ liệu thực tế (Data-driven). Làm chủ quy trình chuyển đổi triển khai ứng dụng từ môi trường Local sang Cloud bằng Container.
* **Về kỹ năng mềm:** Phát triển tư duy giải quyết vấn đề thông qua tự động hóa. Nâng cao khả năng làm việc nhóm trong việc thảo luận và thống nhất các quyết định về kiến trúc hệ thống.