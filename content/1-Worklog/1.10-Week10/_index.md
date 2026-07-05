---
title: "Week 10 Worklog"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---
### Week 10 Objectives:

- Deploy and configure Amazon Cognito User Pool as a centralized identity management and authentication system.
- Establish an email self-sign-up workflow verified through verification codes (OTP).
- Integrate and configure Endpoints security mechanisms using JSON Web Token (JWT) verification tokens via CognitoAuthorizer in the Globals block.
- Audit Endpoints belonging to UserProfileFunction (/profile/init, /profile/me, /profile/avatar-upload-url) to ensure mandatory default JWT authentication requirements from the system.
- Attend the company event on June 27, 2026.

### Tasks to be deployed this week:

| Day | Task | Start Date | Completion Date | Document Source |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| Mon | - Declare AWS::Cognito::UserPool and UserPoolClient resources in the AWS SAM configuration file <br> - Set CognitoUserPoolIdParam parameters and link the ARN directly to the Globals block to create a centralized security gateway | 22/06/2026   | 22/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Tue | - Configure Auto-Verify Email workflows in Cognito to enable automatic verification code delivery services <br> - Write sample code or test the sign-up interface to ensure the system accurately delivers OTP codes to user mailboxes | 23/06/2026   | 23/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Wed | - Configure Amazon API Gateway as the backend connection gateway <br> - Apply global CognitoUserPoolAuthorizer configurations over Profile subsystem paths, making JWT token decryption and validation mandatory | 24/06/2026   | 24/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Thu | - Construct test scenarios simulating the flow: Registration -> Receive Verification Code via Email -> Confirm Account -> Successful Login and receive JWT tokens from Cognito | 25/06/2026   | 25/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Fri | - Proceed with resource updates using the sam deploy command <br> - Review system logs, audit Cognito Authorizer permissions on API Gateway for Profile endpoints, and freeze Week 10 work outcomes | 26/06/2026   | 26/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Sat | - Attend the company Event <br> - Listen to insights from speakers and company members <br> - Learn about Cloud learning methodologies, technical mindset, and AWS research roadmaps <br> - Take notes and consolidate content learned from the Event | 27/06/2026   | 27/06/2026      | Company event |

### Week 10 Results Achieved:

- Initialized and fully configured Amazon Cognito User Pool, providing a robust foundation for application user account management.

- Successfully deployed the automated email verification registration flow, with the system providing stable OTP delivery and correct account activation state handling.

- Successfully configured the API Gateway Cognito Authorizer at a global scope (Globals), ensuring profile management endpoints (/profile/) are rigorously protected by JWT security token decryption mechanisms.

- Successfully tested account creation and Token retrieval from the client side, building a solid identity security foundation for the Ticket Registration and Personal Profile subsystems in the upcoming week.

- Participated in the "FCAJ COMMUNITY DAY" event at the company on June 27, 2026.

- Acquired additional practical experience from speakers and company members regarding Cloud learning methods, technical mindset, and AWS learning direction.
