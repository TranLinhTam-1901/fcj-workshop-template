---
title: "Worklog Tuần 11"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---
### Mục tiêu tuần 11:

- Mở rộng tính năng hệ thống xác thực Amazon Cognito, tích hợp giải pháp đăng nhập qua Google (Google Login OAuth).
- Phát triển mã nguồn trên nền tảng .NET 8 cho UserProfileLambda chịu trách nhiệm xử lý logic nghiệp vụ API lấy thông tin cá nhân và cập nhật thông tin hồ sơ (GET/PUT /profile/me).
- Xây dựng API phát hành đường dẫn tải lên có giới hạn thời gian (S3 Presigned URL) tại endpoint /profile/avatar-upload-url để quản lý việc upload ảnh avatar lên S3 từ Client.
- Phát triển AWS Lambda Function (TicketLambda) trên .NET 8 chịu trách nhiệm xử lý logic nghiệp vụ API đăng ký vé sự kiện, kiểm tra slot trống và đưa vào danh sách chờ (Waiting List).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| 2   | - Cấu hình Google Cloud Console để lấy Client ID và Client Secret cho ứng dụng Web <br> - Khai báo Identity Provider (Google) bên trong cấu hình Amazon Cognito User Pool thông qua tệp SAM Template | 29/06/2026   | 29/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 3   | - Thiết lập thuộc tính ánh xạ (Attribute Mapping) giữa tài khoản Google và Cognito User Pool <br> - Viết mã xử lý đọc context định danh (Cognito Claims) và triển khai logic đồng bộ dữ liệu người dùng vào bảng EventManagementUsers | 30/06/2026   | 30/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 4   | - Viết mã nguồn tích hợp AWS SDK cho .NET tại endpoint /profile/avatar-upload-url nhằm sinh S3 Presigned URL có thời gian hết hạn cố định giúp Client đăng tải trực tiếp file ảnh avatar lên S3 | 01/07/2026   | 01/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| 5   | - Viết mã nguồn .NET 8 cho TicketLambda để lấy thông tin tổng số lượng vé hiện tại của sự kiện từ DynamoDB nhằm tính toán số lượng slot trống <br> - Triển khai logic điều hướng nghiệp vụ: Ghi nhận trạng thái CONFIRMED vào TicketTable hoặc đẩy vào RegistrationTable dưới dạng WAITING_LIST | 02/07/2026   | 02/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| 6   | - Chạy lệnh sam deploy đưa toàn bộ mã nguồn xử lý và cấu hình tích hợp Google lên đám mây <br> - Sử dụng Postman gửi dữ liệu thử nghiệm để kiểm tra tính chính xác của hàm sinh Presigned URL, cập nhật thông tin profile và hàm xử lý đăng ký vé | 03/07/2026   | 03/07/2026      | https://cloudjourney.awsstudygroup.com/ |

### Kết quả đạt được tuần 11:

- Mở rộng thành công cơ chế xác thực của hệ thống, cho phép người dùng đăng nhập linh hoạt bằng tài khoản Google thông qua giao thức OAuth2.

- Phát triển hoàn thiện mã nguồn .NET 8 cho UserProfileLambda, xử lý mượt mà việc đồng bộ thông tin hồ sơ cá nhân với DynamoDB và thiết lập thành công cơ chế sinh Presigned URL để upload ảnh trực tiếp lên Amazon S3.

- Phát triển hoàn thiện AWS Lambda Function chịu trách nhiệm xử lý luồng đăng ký vé sự kiện, kết nối an toàn với cơ sở dữ liệu DynamoDB.

- Xây dựng chính xác thuật toán kiểm tra slot trống theo thời gian thực, xử lý đồng bộ việc phân phối người dùng vào danh sách chính thức hoặc danh sách chờ (Waiting List) dựa trên giới hạn của sự kiện.

- Đóng gói và triển khai thành công mã nguồn phân hệ lên môi trường AWS đám mây bằng công cụ AWS SAM, sẵn sàng cho công tác kiểm thử tích hợp toàn diện.


