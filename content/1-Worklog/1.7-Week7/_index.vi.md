---
title: "Worklog Tuần 7"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

- Nghiên cứu tổng quan đề tài thực tập "Cloud-Based Event Management Platform" và xác định phạm vi nghiệp vụ được giao.
- Nghiên cứu giải pháp Amazon Cognito phục vụ quản lý định danh và phân hệ Xác thực (Authentication).
- Tìm hiểu cấu hình luồng đăng ký tài khoản qua Email có xác thực gửi mã và giải pháp mở rộng đăng nhập bằng Google.
- Tìm hiểu kiến trúc Serverless gồm API Gateway, AWS Lambda và Amazon DynamoDB phục vụ luồng xử lý đăng ký vé sự kiện.
- Phân tích và đánh giá tính khả thi kỹ thuật của các dịch vụ đám mây lựa chọn cho phân hệ đảm nhiệm.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                                                      | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                          |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| 2   | - Nghiên cứu tài liệu tổng quan đề tài "Cloud-Based Event Management Platform" <br> - Phân tích chi tiết các yêu cầu chức năng của phân hệ Auth và Đăng ký vé sự kiện | 01/06/2026   | 01/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 3   | - Tìm hiểu dịch vụ Amazon Cognito User Pool và các thiết lập thuộc tính người dùng <br> - Nghiên cứu cơ chế tự động gửi mã xác thực (Verification Code) qua Email khi người dùng đăng ký | 02/06/2026   | 02/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 4   | - Nghiên cứu tính năng mở rộng xác thực Federated Identities thông qua Hosted UI <br> - Tìm hiểu phương thức cấu hình tích hợp Google Social Login qua giao thức OAuth2 | 03/06/2026   | 03/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 5   | - Tìm hiểu mô hình kiến trúc Serverless cho luồng đăng ký vé sự kiện <br> - Nghiên cứu cách thiết lập API Gateway (REST API), xử lý logic trong AWS Lambda và lưu trữ dữ liệu vào Amazon DynamoDB | 04/06/2026   | 04/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 6   | - Thực hiện phân tích và đánh giá tính khả thi kỹ thuật (Feasibility Study) cho các dịch vụ cấu hình <br> - Trao đổi với các thành viên trong nhóm để thống nhất thiết kế giao tiếp dữ liệu và hoàn thiện báo cáo tuần | 05/06/2026   | 05/06/2026      | https://cloudjourney.awsstudygroup.com/ |

### Kết quả đạt được tuần 7:

- Nắm vững mục tiêu hệ thống và xác định rõ ràng giới hạn phạm vi công việc cá nhân bao gồm cấu phần Auth và Đăng ký vé.

- Hiểu rõ nguyên lý hoạt động của Amazon Cognito User Pool, luồng kích hoạt tài khoản bằng mã xác thực gửi về Email của người dùng.

- Làm chủ giải pháp cấu hình để tích hợp tính năng đăng nhập mở rộng thông qua Google Provider sử dụng giao thức OAuth2.

- Định hình được luồng tương tác dữ liệu từ API Gateway, xử lý nghiệp vụ tại AWS Lambda và quản lý trạng thái đăng ký vé, danh sách chờ trong DynamoDB.

- Hoàn thành tài liệu phân tích tính khả thi kỹ thuật, đảm bảo hạ tầng Serverless đề xuất đáp ứng tốt yêu cầu về bảo mật và khả năng vận hành.


