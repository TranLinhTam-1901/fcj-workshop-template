---
title: "Worklog Tuần 10"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---
### Mục tiêu tuần 10:

- Triển khai và cấu hình Amazon Cognito User Pool làm hệ thống quản lý định danh và xác thực tập trung.
- Thiết lập luồng đăng ký tài khoản tự phục vụ (Self-Sign-Up) bằng Email có xác thực thông qua mã Verification Code (OTP).
- Tích hợp và cấu hình cơ chế bảo mật Endpoints sử dụng mã xác thực dạng JSON Web Token (JWT) thông qua CognitoAuthorizer tại khối Globals.
- Rà soát các Endpoint thuộc UserProfileFunction (/profile/init, /profile/me, /profile/avatar-upload-url) để đảm bảo yêu cầu xác thực JWT mặc định bắt buộc từ hệ thống.
- Tham gia Event tại công ty vào 27/06/2026.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| 2   | - Khai báo tài nguyên AWS::Cognito::UserPool và UserPoolClient trong tệp cấu hình AWS SAM <br> - Thiết lập thuộc tính tham số CognitoUserPoolIdParam và liên kết trực tiếp ARN vào khối Globals để tạo cổng bảo mật tập trung | 22/06/2026   | 22/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 3   | - Cấu hình luồng Auto-Verify Email trong Cognito để kích hoạt dịch vụ tự động gửi mã xác thực (Verification Code) <br> - Viết mã mẫu hoặc kiểm thử giao diện đăng ký để đảm bảo hệ thống gửi mã OTP về hòm thư người dùng chính xác | 23/06/2026   | 23/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 4   | - Cấu hình Amazon API Gateway làm cổng kết nối cho các dịch vụ Backend <br> - Áp dụng CognitoUserPoolAuthorizer toàn cục lên các tuyến đường của phân hệ Profile, bắt buộc phải giải mã và kiểm tra tính hợp lệ của JWT Token | 24/06/2026   | 24/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 5   | - Thực hiện xây dựng các kịch bản kiểm thử giả lập luồng Đăng ký -> Nhận mã Verification Code qua Email -> Xác nhận tài khoản -> Đăng nhập thành công và nhận mã JWT từ Cognito | 25/06/2026   | 25/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 6   | - Tiến hành triển khai bản cập nhật tài nguyên bằng lệnh sam deploy <br> - Rà soát log hệ thống, kiểm tra quyền hạn của Cognito Authorizer trên API Gateway đối với các Endpoint của Profile và chốt kết quả công việc tuần 10 | 26/06/2026   | 26/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 7   | - Tham gia buổi Event tại công ty <br> - Lắng nghe chia sẻ từ diễn giả và các thành viên công ty <br> - Tìm hiểu cách học Cloud, tư duy kỹ thuật và định hướng nghiên cứu AWS <br> - Ghi chú và tổng hợp nội dung học được từ Event | 27/06/2026   | 27/06/2026      | Company event |

### Kết quả đạt được tuần 10:

- Khởi tạo và cấu hình hoàn chỉnh Amazon Cognito User Pool, làm nền tảng vững chắc cho việc quản lý tài khoản người dùng của ứng dụng.

- Triển khai thành công luồng đăng ký tài khoản tự động xác thực bằng Email, hệ thống gửi mã OTP ổn định và xử lý kích hoạt trạng thái tài khoản chính xác.

- Cấu hình thành công API Gateway Cognito Authorizer ở phạm vi toàn cục (Globals), đảm bảo các endpoint quản lý hồ sơ cá nhân (/profile/) được bảo vệ nghiêm ngặt bằng cơ chế giải mã mã bảo mật JWT.

- Kiểm thử thành công luồng tạo tài khoản và lấy Token từ phía Client, làm cơ sở bảo mật thông tin định danh cho phân hệ Đăng ký vé và Hồ sơ cá nhân ở tuần kế tiếp.

- Tham gia Event "FCAJ COMMUNITY DAY" tại công ty vào ngày 27/06/2026.

- Tiếp thu thêm kinh nghiệm thực tế từ diễn giả và các thành viên công ty về phương pháp học Cloud, tư duy kỹ thuật và định hướng học AWS.



