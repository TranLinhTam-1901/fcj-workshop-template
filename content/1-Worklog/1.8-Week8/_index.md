---
title: "Week 8 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---
### Week 8 Objectives:

- Analyze system requirements in detail and clearly define the Minimum Viable Product (MVP) scope for the assigned individual components.
- Design detailed User Flow diagrams for the Authentication subsystem using Amazon Cognito.
- Design User Flow diagrams for the event ticket registration business logic, including handling scenarios for the Waiting List.
- Sketch the overall Serverless architecture model to prepare for the infrastructure deployment phase in the following week.

### Tasks to be deployed this week:

| Day | Task | Start Date | Completion Date | Document Source |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------- |
| Mon | - Analyze Use Cases for the Auth and Ticket Registration subsystems <br> - Identify core criteria within the MVP scope such as: Email Sign-Up/Sign-In, Google Login, Ticket Registration, and Empty Slot handling | 08/06/2026   | 08/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Tue | - Design User Flows for the authentication process: Account Sign-Up -> Input OTP/Verification Code sent via Email to activate the account <br> - Construct the direct sign-in flow via Google OAuth and map information into the Cognito User Pool | 09/06/2026   | 09/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Wed | - Design User Flows for the ticket registration process: Check available slots -> Save valid registration information or change status to Waiting List if slots are full | 10/06/2026   | 10/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Thu | - Model the overall Serverless architecture for the assigned subsystem <br> - Define security integration flows: Utilize JWT tokens from Cognito as an Authorizer to protect ticket registration endpoints on API Gateway | 11/06/2026   | 11/06/2026      | https://cloudjourney.awsstudygroup.com/ |
| Fri | - Conduct team meetings to review and optimize the designed user flow diagrams <br> - Cross-check with members in charge of other modules to ensure data synchronization and freeze the Week 8 design documentation | 12/06/2026   | 12/06/2026      | Technical team meeting |

### Week 8 Results Achieved:

- Completed MVP scope definition clearly, helping to optimize deployment timelines for core project features.

- Successfully built User Flow diagrams for the Authentication subsystem, covering detailed email OTP verification flows and Google account linking workflows.

- Finalized business user flows for event ticket registration, covering all scenarios from successful registration to automatic assignment into the Waiting List.

- Established the overall Serverless architecture blueprint, clearly defining the API security method using the Cognito JWT Authorizer solution before handing off data to the Lambda processing layer and DynamoDB storage.

- Synchronized individual designs with the group's overall structure, ensuring readiness in documentation and logical thinking to initiate actual cloud infrastructure setup next week.
