---
title: "Worklog Tuần 4"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---
### Mục tiêu tuần 4:

- Hiểu các khái niệm cơ bản về dịch vụ tính toán và lưu trữ trên AWS.
- Tìm hiểu các thành phần chính của Amazon EC2 như instance type, AMI, key pair, security group và EBS volume.
- Tìm hiểu các dịch vụ lưu trữ như Amazon EFS và Amazon FSx.
- Nắm được mục đích cơ bản của AWS Application Migration Service (AWS MGN).
- Hiểu cách EC2 Auto Scaling hỗ trợ mở rộng hệ thống và tăng tính sẵn sàng.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                     | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                          |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| 2   | - Tìm hiểu Amazon EC2 cơ bản <br>  + EC2 instance <br>  + AMI <br>  + Instance type <br>  + Key pair <br>  + Security Group <br> - Hiểu các trường hợp sử dụng EC2 để chạy máy chủ ảo trên AWS                                | 11/05/2026   | 11/05/2026      | https://cloudjourney.awsstudygroup.com/ |
| 3   | - Tìm hiểu các lựa chọn lưu trữ cho EC2 <br>  + Amazon EBS <br>  + Các loại EBS volume <br>  + Snapshot <br> - Tìm hiểu cách EBS được gắn vào EC2 instance <br> - Ghi chú mối quan hệ giữa EC2 và EBS                         | 12/05/2026   | 12/05/2026      | https://cloudjourney.awsstudygroup.com/ |
| 4   | - Tìm hiểu các dịch vụ lưu trữ chia sẻ trên AWS <br>  + Amazon EFS <br>  + Amazon FSx <br> - So sánh trường hợp sử dụng cơ bản giữa EBS, EFS và FSx <br> - Hiểu khi nào cần sử dụng shared file storage trong kiến trúc Cloud | 13/05/2026   | 13/05/2026      | https://cloudjourney.awsstudygroup.com/ |
| 5   | - Tìm hiểu AWS Application Migration Service (AWS MGN) <br> - Hiểu ý tưởng cơ bản của việc di chuyển máy chủ và workload lên AWS <br> - Ghi chú các khái niệm migration như source server, replication, cutover và testing    | 14/05/2026   | 14/05/2026      | https://cloudjourney.awsstudygroup.com/ |
| 6   | - Tìm hiểu EC2 Auto Scaling <br>  + Launch Template <br>  + Auto Scaling Group <br>  + Scaling policy <br> - Hiểu cách Auto Scaling hỗ trợ high availability và cost optimization <br> - Tổng hợp nội dung đã học trong tuần  | 15/05/2026   | 15/05/2026      | https://cloudjourney.awsstudygroup.com/ |

### Kết quả đạt được tuần 4:

- Hiểu được vai trò cơ bản của Amazon EC2 là dịch vụ tính toán dùng để chạy máy chủ ảo trên AWS.

- Nắm được các thành phần chính của EC2:
  - EC2 instance
  - Amazon Machine Image (AMI)
  - Instance type
  - Key pair
  - Security Group
  - Elastic Block Store (EBS)

- Hiểu cách Amazon EBS cung cấp block storage cho EC2 instance và cách snapshot được sử dụng cho mục đích sao lưu.

- Phân biệt được cơ bản các dịch vụ lưu trữ trên AWS:
  - Amazon EBS cho block storage
  - Amazon EFS cho shared file storage
  - Amazon FSx cho managed file system

- Hiểu mục đích của AWS Application Migration Service (AWS MGN) trong việc di chuyển máy chủ và workload từ môi trường on-premises hoặc môi trường khác lên AWS.

- Nắm được một số khái niệm cơ bản liên quan đến migration:
  - Source server
  - Replication
  - Test launch
  - Cutover
  - Migration lifecycle

- Hiểu cách EC2 Auto Scaling giúp ứng dụng duy trì tính sẵn sàng và tự động điều chỉnh tài nguyên theo nhu cầu sử dụng.

- Nhận thức được mối liên hệ giữa scalability, availability và cost optimization khi thiết kế hệ thống Cloud.

- Hoàn thành ghi chú và tổng hợp kiến thức về compute, storage, migration và scaling để chuẩn bị cho các bài thực hành ở những tuần tiếp theo.



