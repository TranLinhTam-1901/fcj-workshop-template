---
title: "Week 9 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---
### Week 9 Objectives:

- Initialize the Serverless infrastructure foundation for the project using the AWS Serverless Application Model (AWS SAM) tool.
- Initialize and configure NoSQL databases with Amazon DynamoDB serving the ticket registration subsystem (RegistrationTable, TicketTable) and personal profile storage (EventManagementUsers).
- Configure Amazon S3 storage resources (EventManagementUserAvatarsBucket) to store user avatars.
- Design and delegate security permissions using AWS IAM Roles, applying integrated policies (DynamoDBCrudPolicy, S3CrudPolicy) adhering to the principle of Least Privilege.
- Deploy and test Infrastructure as Code (IaC) source code on the personal AWS Cloud environment to verify correctness.

### Tasks to be deployed this week:

| Day | Task | Start Date | Completion Date | Document Source |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| Mon | - Install and configure the local development environment with AWS SAM CLI <br> - Write the initial foundation template.yaml file defining project details and basic environment variables | 15/06/2026   | 15/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Tue | - Initialize the database structures within the SAM configuration file for data tables: RegistrationTable, TicketTable, and the user table EventManagementUsers <br> - Define appropriate Partition Keys and Sort Keys properties | 16/06/2026   | 16/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Wed | - Declare structures for the storage system EventManagementUserAvatarsBucket on S3 <br> - Configure CORS rules (AllowedMethods: PUT, GET) for the Bucket to prepare infrastructure for direct avatar uploads from Frontend | 17/06/2026   | 17/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Thu | - Establish AWS IAM Roles and IAM Policies defining access rights <br> - Configure strict permissions allowing the Lambda function handling personal profiles (UserProfileLambda) to have read/write privileges on the corresponding DynamoDB tables and S3 Buckets | 18/06/2026   | 18/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Fri | - Execute sam build and sam deploy --guided commands to deploy infrastructure from local to AWS Cloud via CloudFormation <br> - Verify resource status on the AWS Console, audit configuration errors, and close Week 9 results | 19/06/2026   | 19/06/2026      | https://cloudjourney.awsstudygroup.com/ |

### Week 9 Results Achieved:

- Successfully established the Infrastructure as Code (IaC) development environment with AWS SAM, directly serving infrastructure code management.

- Successfully initialized NoSQL databases on Amazon DynamoDB, including **RegistrationTable**, **TicketTable**, and the user profile management table **EventManagementUsers** with optimal Key structures for querying.

- Completely configured the Amazon S3 Bucket dedicated to user avatars, pre-integrating required CORS policies to be ready for client application upload flows.

- Built a secure authorization system via AWS IAM Roles, ensuring proper control of internal connections between services and least privileges for Lambda functions.

- Successfully deployed all foundational resources to the AWS account via CloudFormation without errors, with resources displaying correct operational status on the AWS Management Console.

- Prepared a solid storage infrastructure foundation to enter the user authentication setup phase in the following week.