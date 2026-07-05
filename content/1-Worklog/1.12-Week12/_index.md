---
title: "Week 12 Worklog"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.12. </b> "
---
### Week 12 Objectives:

- Perform End-to-End integration linking assigned personal subsystems including Authentication workflows (Cognito), Personal Profile management with avatar upload (Profile/S3), and Ticket Registration (Lambda/DynamoDB).
- Conduct full-system Integration Testing to detect and resolve emerging errors.
- Perform review and optimization of operational costs for configured Serverless resources (AWS Budgets, DynamoDB Capacity, Lambda Timeout).
- Finalize technical documentation (Workshop Report), package infrastructure source codes, and prepare for project handoff.

### Tasks to be deployed this week:

| Day | Task | Start Date | Completion Date | Document Source |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| Mon | - Execute End-to-End synchronization configuration: Append JWT tokens acquired after Login into request Headers <br> - Run full integration scenarios: Log in -> Fetch Presigned URL -> Upload photos to S3 -> Update Profile -> Send ticket registration API | 06/07/2026   | 06/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| Tue | - Write scripts and perform system integration testing across diverse data variants to verify the stability of API Gateway Authorizers, waiting list processing Lambdas, and personal profile subsystems | 07/07/2026   | 07/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| Wed | - Review cloud resource configurations to optimize costs: Convert DynamoDB to On-demand mode, adjust allocated memory sizes for Lambdas, and configure appropriate log retention times on CloudWatch | 08/07/2026   | 08/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| Thu | - Consolidate and finalize the detailed final-term technical document (Workshop Report) covering authentication architectures, S3 personal profile modules, and event ticket registration modules <br> - Package SAM Template infrastructure code to the team repository | 09/07/2026   | 09/07/2026      | https://cloudjourney.awsstudygroup.com/ |
| Fri | - Conduct an overall review of all resources on the AWS account <br> - Hand over source codes and project documentation to the internship mentor at the enterprise, officially concluding the internship period | 10/07/2026   | 10/07/2026      | https://cloudjourney.awsstudygroup.com/ |

### Week 12 Results Achieved:

- Successfully integrated complete business workflows (End-to-End): Users log in via Email/Google, receive secure JWT Tokens to update profile details, upload avatar files to S3, and register for event tickets securely.

- Completed the full-system integration testing process, thoroughly resolving access permission errors at the API Gateway Authorizer, ensuring profile updates and operational logistics run smoothly.

- Successfully optimized Serverless application performance leveraging the .NET 8 environment and managed cloud operational costs based on AWS best practices.

- Completed full technical handoff documentation (Workshop Report) and packaged Infrastructure as Code (IaC) architectures cleanly and systematically.

- Fulfilled all initial objectives set for the internship program, successfully completing assigned component development tasks within the project and executing product handoff right on schedule.
