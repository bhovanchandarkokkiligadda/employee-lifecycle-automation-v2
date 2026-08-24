# Testing & Validation

## Purpose

This document describes the testing approach used to validate the ServiceNow Employee Lifecycle Automation application.

## Functional Testing

### Employee Onboarding

Verify that:

- The onboarding catalog item is available.
- Required fields are validated.
- A request is created after submission.
- The request receives a unique number.
- The approval process is triggered.
- Required tasks are generated after approval.
- Notifications are generated.
- The request can reach completion.

### Employee Offboarding

Verify that:

- The offboarding catalog item is available.
- Required information is collected.
- A request is created successfully.
- Approval is triggered.
- Offboarding tasks are generated.
- Notifications are generated.
- The request can be completed.

## Workflow Testing

Validate the complete lifecycle:

```mermaid
graph TD
    A[Request Submitted] --> B[Approval Requested]
    B --> C[Approved]
    C --> D[Tasks Created]
    D --> E[Tasks Assigned]
    E --> F[Tasks Completed]
    F --> G[Request Completed]
