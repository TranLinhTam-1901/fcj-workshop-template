---
title: "Worklog Tuần 8"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---
### Mục tiêu tuần 8:

- Phân tích chi tiết các yêu cầu hệ thống và xác định rõ ràng phạm vi sản phẩm khả dụng tối thiểu (MVP) đối với các cấu phần cá nhân phụ trách.
- Thiết kế sơ đồ luồng người dùng (User Flow) chi tiết cho phân hệ Xác thực (Authentication) sử dụng Amazon Cognito.
- Thiết kế sơ đồ luồng người dùng (User Flow) cho nghiệp vụ đăng ký vé sự kiện, bao gồm cả trường hợp xử lý danh sách chờ (Waiting List).
- Phác thảo mô hình kiến trúc Serverless tổng thể để chuẩn bị cho giai đoạn triển khai hạ tầng ở tuần tiếp theo.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                                                      | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                          |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| 2   | - Phân tích các ca sử dụng (Use Cases) cho phân hệ Auth và Đăng ký vé <br> - Xác định các tiêu chí cốt lõi thuộc phạm vi MVP như: Đăng ký/Đăng nhập bằng Email, Login qua Google, Đăng ký vé sự kiện và xử lý Slot trống | 08/06/2026   | 08/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 3   | - Thiết kế sơ đồ User Flow cho luồng xác thực: Đăng ký tài khoản -> Nhập mã OTP/Verification Code gửi qua Email để kích hoạt tài khoản <br> - Xây dựng luồng đăng nhập trực tiếp qua Google OAuth và ánh xạ thông tin vào Cognito User Pool | 09/06/2026   | 09/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 4   | - Thiết kế sơ đồ User Flow cho luồng đăng ký vé sự kiện: Kiểm tra số lượng slot khả dụng -> Lưu thông tin đăng ký hợp lệ hoặc chuyển trạng thái sang Waiting List nếu hết slot | 10/06/2026   | 10/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 5   | - Mô hình hóa kiến trúc Serverless tổng thể cho phân hệ đảm nhiệm <br> - Xác định luồng tích hợp bảo mật: Sử dụng mã thông báo JWT từ Cognito làm Authorizer bảo vệ các endpoints đăng ký vé trên API Gateway | 11/06/2026   | 11/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| 6   | - Tổ chức họp nhóm để rà soát, tối ưu hóa các sơ đồ luồng người dùng đã thiết kế <br> - Đối chiếu lại với các thành viên phụ trách Module khác nhằm đảm bảo tính đồng bộ dữ liệu và chốt tài liệu thiết kế tuần 8 | 12/06/2026   | 12/06/2026      | Họp nhóm kỹ thuật |

### Kết quả đạt được tuần 8:

- Hoàn thành việc xác định phạm vi MVP một cách rõ ràng, giúp tối ưu hóa thời gian triển khai các tính năng cốt lõi cho dự án.

- Xây dựng thành công sơ đồ luồng người dùng (User Flow) cho phân hệ Xác thực, bao gồm chi tiết luồng kiểm tra mã OTP qua Email và luồng liên kết tài khoản Google.

- Hoàn thiện sơ đồ luồng nghiệp vụ đăng ký vé sự kiện, bao phủ toàn bộ các kịch bản từ đăng ký thành công cho đến việc tự động phân phối vào danh sách chờ (Waiting List).

- Thiết lập bản vẽ kiến trúc Serverless tổng thể, định hình rõ ràng phương án bảo mật API bằng giải pháp Cognito JWT Authorizer trước khi chuyển giao thông tin sang tầng xử lý Lambda và lưu trữ DynamoDB.

- Đồng bộ hóa thiết kế cá nhân với cấu trúc tổng thể của cả nhóm, sẵn sàng về mặt tài liệu và tư duy logic để bắt đầu khởi tạo hạ tầng đám mây thực tế ở tuần sau.


