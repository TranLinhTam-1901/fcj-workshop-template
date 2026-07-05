---
title: "Worklog Tuần 9"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---
### Mục tiêu tuần 9:

- Khởi tạo nền tảng hạ tầng Serverless cho dự án bằng công cụ AWS Serverless Application Model (AWS SAM).
- Khởi tạo và cấu hình cơ sở dữ liệu NoSQL với Amazon DynamoDB phục vụ cho phân hệ đăng ký vé (RegistrationTable, TicketTable) và lưu trữ thông tin hồ sơ cá nhân (EventManagementUsers).
- Cấu hình tài nguyên lưu trữ Amazon S3 (EventManagementUserAvatarsBucket) để lưu avatar người dùng.
- Thiết kế và phân quyền bảo mật bằng AWS IAM Roles, áp dụng các chính sách tích hợp (DynamoDBCrudPolicy, S3CrudPolicy), tuân thủ nguyên tắc đặc quyền tối thiểu (Least Privilege).
- Triển khai thử nghiệm mã nguồn hạ tầng dạng mã (IaC) lên môi trường AWS Cloud cá nhân để kiểm tra tính đúng đắn.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| 2   | - Cài đặt và cấu hình môi trường phát triển tại local với AWS SAM CLI <br> - Viết file cấu hình nền tảng ban đầu template.yaml định nghĩa thông tin project và các thông số môi trường cơ bản | 15/06/2026   | 15/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 3   | - Khởi tạo cấu trúc cơ sở dữ liệu trên tệp cấu hình SAM cho bảng dữ liệu: RegistrationTable, TicketTable và bảng người dùng EventManagementUsers <br> - Định nghĩa các thuộc tính Khóa chính (Partition Key) và Khóa sắp xếp (Sort Key) phù hợp | 16/06/2026   | 16/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 4   | - Khai báo cấu trúc cho hệ thống lưu trữ EventManagementUserAvatarsBucket trên S3 <br> - Cấu hình quy tắc CORS (AllowedMethods: PUT, GET) cho Bucket nhằm chuẩn bị hạ tầng phục vụ cơ chế tải ảnh đại diện trực tiếp từ phía Frontend | 17/06/2026   | 17/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 5   | - Thiết lập AWS IAM Roles và IAM Policies quy định quyền hạn truy cập <br> - Cấu hình phân quyền chặt chẽ cho phép hàm Lambda xử lý hồ sơ cá nhân (UserProfileLambda) có đặc quyền đọc/ghi dữ liệu vào bảng DynamoDB và S3 Bucket tương ứng | 18/06/2026   | 18/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 6   | - Thực hiện lệnh sam build và sam deploy --guided để triển khai hạ tầng từ local lên AWS Cloud thông qua CloudFormation <br> - Kiểm tra trạng thái tài nguyên trên AWS Console, rà soát lỗi cấu hình và chốt kết quả tuần 9 | 19/06/2026   | 19/06/2026      | https://cloudjourney.awsstudygroup.com/ |

### Kết quả đạt được tuần 9:

- Thiết lập thành công môi trường phát triển Infrastructure as Code (IaC) với AWS SAM phục vụ trực tiếp cho việc quản lý mã nguồn hạ tầng.

- Khởi tạo thành công các bảng dữ liệu NoSQL trên Amazon DynamoDB bao gồm **RegistrationTable**, **TicketTable** và bảng quản lý hồ sơ người dùng **EventManagementUsers** với cấu trúc Khóa tối ưu cho việc truy vấn.

- Cấu hình hoàn chỉnh Amazon S3 Bucket dành cho ảnh đại diện, tích hợp sẵn các chính sách CORS cần thiết để sẵn sàng cho luồng Upload ảnh từ ứng dụng Client.

- Xây dựng hệ thống phân quyền an toàn thông qua AWS IAM Roles, đảm bảo kiểm soát tốt các kết nối nội bộ giữa các dịch vụ và đặc quyền tối thiểu của các hàm Lambda.

- Triển khai (Deploy) thành công toàn bộ tài nguyên nền tảng lên tài khoản AWS thông qua CloudFormation mà không gặp lỗi, các tài nguyên hiển thị đúng trạng thái hoạt động trên AWS Management Console.

- Sẵn sàng cơ sở hạ tầng lưu trữ vững chắc để bước vào giai đoạn cấu hình hệ thống Xác thực người dùng ở tuần tiếp theo.


