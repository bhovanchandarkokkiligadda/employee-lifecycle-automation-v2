

# ServiceNow Employee Lifecycle Automation

## Project Overview

ServiceNow Employee Lifecycle Automation is an employee onboarding and offboarding management system built on the ServiceNow platform.

The application uses Service Catalog, dynamic forms, Flow Designer automation, approvals, task management, SLA monitoring, notifications, role-based access, and employee lifecycle tracking.

## Business Objective

The objective of the application is to streamline employee onboarding and offboarding activities through a centralized ServiceNow workflow.

The system helps coordinate employees, managers, HR teams, and other responsible users while maintaining workflow visibility and traceability.

## Core Features

- Employee onboarding request
- Employee offboarding request
- Service Catalog integration
- Dynamic employee lifecycle forms
- Approval workflows
- Flow Designer automation
- Automatic task creation
- Task assignment and tracking
- SLA monitoring
- Notifications
- Employee lifecycle tracking
- Role-based access control
- Dashboard and monitoring capabilities
- Source-controlled application configuration
- Update set and deployment history

## Employee Onboarding Flow

Employee Onboarding Request
          ↓
Service Catalog Submission
          ↓
Request Validation
          ↓
Approval
          ↓
Task Creation
          ↓
Task Assignment
          ↓
Task Completion
          ↓
Request Completion


## Employee Offboarding Flow

Employee Offboarding Request
          ↓
Service Catalog Submission
          ↓
Request Validation
          ↓
Approval
          ↓
Offboarding Tasks
          ↓
Task Assignment
          ↓
Task Completion
          ↓
Request Closure

## Automation

Flow Designer is used to automate important lifecycle activities such as:

* Request processing
* Approval handling
* Task generation
* Task assignment
* Notifications
* Lifecycle status management

## SLA Management

SLA monitoring is included to help track lifecycle tasks and ensure that activities are completed within defined service targets.

## Notifications

Notifications provide updates to relevant users during important stages of the employee lifecycle.

Examples include:

* Request submission
* Approval requests
* Approval results
* Task assignments
* Task completion
* Request completion

## Security

Role-based access controls are used to restrict access to application functionality and employee lifecycle information.

The application is designed to ensure that users can perform only the activities appropriate to their assigned roles.

## Source Control

The application is connected to GitHub through ServiceNow Studio Source Control.

The source-control workflow includes:

ServiceNow
    ↓
Source Control Commit
    ↓
GitHub Development Branch
    ↓
Pull Request
    ↓
Validation
    ↓
main Branch

## Testing

The application is validated through functional and end-to-end testing of:

* Service Catalog requests
* Onboarding workflow
* Offboarding workflow
* Approvals
* Task generation
* SLA monitoring
* Notifications
* Role-based access
* Request completion

## Demo

The application demonstration covers:

1. Service Catalog navigation
2. HR Services
3. Employee onboarding/offboarding request
4. Request submission
5. Approval workflow
6. Task creation
7. SLA monitoring
8. Notifications
9. Request completion

## Repository Structure

employee-lifecycle-automation-v2/
│
├── docs/
│   ├── architecture.md
│   ├── demo-guide.md
│   ├── deployment.md
│   ├── setup-guide.md
│   └── testing.md
│
├── project-report/
│   └── project-report.md
│
├── screenshots/
│
├── update-set/
│
├── README.md
└── sn_source_control.properties

## Conclusion

The ServiceNow Employee Lifecycle Automation application provides a structured approach to managing employee onboarding and offboarding activities.

By combining Service Catalog, Flow Designer, approvals, tasks, SLAs, notifications, security, and source control, the application provides an auditable and organized employee lifecycle management workflow.



