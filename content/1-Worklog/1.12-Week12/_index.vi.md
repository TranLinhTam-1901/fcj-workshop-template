---
title: "Worklog Tuần 12"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.12 </b> "
---
### Mục tiêu tuần 12:

- Tích hợp liên thông các phân hệ cá nhân đảm nhiệm bao gồm luồng Xác thực (Cognito), Quản lý hồ sơ cá nhân kèm tải ảnh đại diện (Profile/S3) và Đăng ký vé (Lambda/DynamoDB) theo mô hình End-to-End.
- Tiến hành kiểm thử liên thông (Integration Testing) toàn hệ thống để phát hiện và xử lý các lỗi phát sinh.
- Thực hiện rà soát, tối ưu hóa chi phí vận hành các tài nguyên Serverless đã cấu hình (AWS Budgets, DynamoDB Capacity, Lambda Timeout).
- Hoàn thiện tài liệu kỹ thuật (Workshop Report), đóng gói mã nguồn hạ tầng và chuẩn bị bàn giao dự án.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| 2   | - Thực hiện cấu hình đồng bộ End-to-End: Gắn mã xác thực JWT nhận được sau khi Login vào Header của yêu cầu <br> - Thực hiện kịch bản liên thông đầy đủ: Đăng nhập -> Lấy Presigned URL -> Upload ảnh lên S3 -> Cập nhật Profile -> Gửi API đăng ký vé sự kiện | 06/07/2026   | 06/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| 3   | - Tiến hành viết kịch bản và thực hiện kiểm thử liên thông hệ thống với nhiều trường hợp dữ liệu khác nhau để kiểm tra độ ổn định của API Gateway Authorizer, hàm Lambda xử lý danh sách chờ và phân hệ quản lý hồ sơ cá nhân | 07/07/2026   | 07/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| 4   | - Rà soát cấu hình tài nguyên đám mây để tối ưu hóa chi phí: Chuyển đổi DynamoDB sang dạng On-demand, điều chỉnh dung lượng bộ nhớ phù hợp cho Lambda và cấu hình thời gian lưu trữ log hợp lý trên CloudWatch | 08/07/2026   | 08/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| 5   | - Tổng hợp và hoàn thiện cuốn tài liệu kỹ thuật cuối kỳ (Workshop Report) chi tiết về kiến trúc hệ thống xác thực, module hồ sơ cá nhân S3 và module đăng ký vé sự kiện <br> - Đóng gói mã nguồn hạ tầng SAM Template lên kho lưu trữ chung của nhóm | 09/07/2026   | 09/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| 6   | - Thực hiện rà soát tổng thể toàn bộ tài nguyên trên tài khoản AWS <br> - Tiến hành bàn giao mã nguồn, tài liệu dự án cho người hướng dẫn thực tập tại doanh nghiệp và chính thức khép lại kỳ thực tập | 10/07/2026   | 10/07/2026      | https://cloudjourney.awsstudygroup.com/ |

### Kết quả đạt được tuần 12:

- Tích hợp thành công luồng nghiệp vụ trọn vẹn (End-to-End): Người dùng đăng nhập qua Email/Google, nhận JWT Token bảo mật để cập nhật thông tin hồ sơ cá nhân, upload ảnh avatar lên S3 và thực hiện đăng ký vé sự kiện một cách an toàn.

- Hoàn thành quá trình kiểm thử liên thông toàn hệ thống, xử lý triệt để các lỗi phân quyền truy cập tại API Gateway Authorizer, bảo đảm logic cập nhật thông tin cá nhân và nghiệp vụ vận hành mượt mà.

- Tối ưu hóa thành công hiệu năng ứng dụng Serverless dựa trên môi trường .NET 8 và cấu trúc chi phí vận hành đám mây dựa trên các best practices của AWS.

- Hoàn thiện đầy đủ bộ tài liệu kỹ thuật bàn giao (Workshop Report), đóng gói mã nguồn hạ tầng dạng mã (IaC) rõ ràng, khoa học.

- Đạt được toàn bộ các mục tiêu đặt ra ban đầu của kỳ thực tập, hoàn thành tốt nhiệm vụ phát triển cấu phần phân công trong dự án và thực hiện bàn giao sản phẩm đúng thời hạn.


