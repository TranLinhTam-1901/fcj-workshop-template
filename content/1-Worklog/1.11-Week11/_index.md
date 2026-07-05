---
title: "Week 11 Worklog"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---
### Week 11 Objectives:

- Extend Amazon Cognito authentication functionalities, integrating solutions to log in via Google (Google Login OAuth).
- Develop .NET 8 source code for UserProfileLambda, responsible for handling business logic APIs to get personal information and update profiles (GET/PUT /profile/me).
- Build a time-limited upload URL issuance API (S3 Presigned URL) at the /profile/avatar-upload-url endpoint to manage avatar uploads to S3 from Clients.
- Develop an AWS Lambda Function (TicketLambda) on .NET 8, responsible for processing event ticket registration business logic, validating empty slots, and putting users into the Waiting List.

### Tasks to be deployed this week:

| Day | Task | Start Date | Completion Date | Document Source |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| Mon | - Configure Google Cloud Console to acquire Client ID and Client Secret for the Web application <br> - Declare Identity Provider (Google) inside the Amazon Cognito User Pool configurations using the SAM Template file | 29/06/2026   | 29/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Tue | - Set up Attribute Mapping between Google accounts and the Cognito User Pool <br> - Write code to read identity contexts (Cognito Claims) and implement user data synchronization logic into the EventManagementUsers table | 30/06/2026   | 30/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Wed | - Write integration source code utilizing AWS SDK for .NET at the /profile/avatar-upload-url endpoint to generate S3 Presigned URLs with fixed expiration times, allowing clients to upload avatar image files directly to S3 | 01/07/2026   | 01/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| Thu | - Write .NET 8 source code for TicketLambda to fetch current total ticket counts of an event from DynamoDB to calculate empty slots <br> - Implement workflow routing logic: Record CONFIRMED status into TicketTable or push to RegistrationTable as WAITING_LIST | 02/07/2026   | 02/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| Fri | - Run sam deploy to deliver all processing source codes and Google integration configurations to the cloud <br> - Use Postman to send test data to verify the accuracy of Presigned URL generation, profile updates, and ticket registration logic functions | 03/07/2026   | 03/07/2026      | https://cloudjourney.awsstudygroup.com/ |

### Week 11 Results Achieved:

- Successfully extended system authentication mechanisms, allowing users to log in flexibly using Google accounts through the OAuth2 protocol.

- Completed .NET 8 source code development for UserProfileLambda, smoothly processing personal profile synchronization with DynamoDB and successfully establishing Presigned URL generation mechanisms for uploading photos directly to Amazon S3.

- Completed AWS Lambda Function development responsible for the event ticket registration pipeline, connecting securely with the DynamoDB database.

- Built accurate real-time empty slot validation algorithms, synchronously managing user placement into formal entry lists or waiting lists (Waiting List) based on event capacity.

- Successfully packaged and deployed subsystem source codes onto the AWS cloud environment using the AWS SAM tool, ready for comprehensive integration testing.
