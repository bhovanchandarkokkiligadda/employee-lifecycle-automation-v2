# Employee Lifecycle Automation on ServiceNow

## 1. Project Overview

The Employee Lifecycle Automation system is a ServiceNow-based application designed to manage employee onboarding and offboarding requests through a centralized and automated workflow.

The application uses ServiceNow Service Catalog, Flow Designer, approvals, task management, SLA configuration, notifications, role-based access, and employee lifecycle tracking to provide a structured process from request submission through completion.

The project also uses ServiceNow Studio Source Control with GitHub to maintain application source code and development history.

---

## 2. Project Objectives

The main objectives of the project are:

- Automate employee onboarding and offboarding processes.
- Provide a centralized Service Catalog request interface.
- Capture employee lifecycle information through structured forms.
- Apply different processing logic based on request type.
- Automate approval processing.
- Generate and manage lifecycle-related tasks.
- Track request and task status.
- Apply SLA monitoring to lifecycle activities.
- Send notifications for important workflow events.
- Provide role-based access to application functionality.
- Maintain traceability of configuration changes through source control.
- Provide a documented and repeatable deployment process.

---

## 3. Application Scope

The application covers the following employee lifecycle activities:

### Employee Onboarding

Onboarding requests can be submitted for newly joining employees.

The request captures employee information and initiates the configured approval and automation process.

### Employee Offboarding

Offboarding requests can be submitted when an employee leaves the organization.

The process can be used to initiate the required employee exit activities and track their completion.

---

## 4. Service Catalog

The application provides an Employee Lifecycle Request catalog item.

### Catalog Item

**Employee Lifecycle Request**

Purpose:

> Submit an employee onboarding or offboarding request.

The catalog item provides a structured request form where users can enter employee lifecycle information.

The form includes fields such as:

- Request Type
- Employee Name
- Employee ID
- Department
- Manager
- Exit Date
- Additional Comments

Some fields are displayed or used depending on the selected request type.

---

## 5. Service Portal

The application is accessible through the ServiceNow Service Portal.

The Service Portal provides the user-facing interface for accessing the Service Catalog and submitting employee lifecycle requests.

The portal allows users to:

- Browse the Service Catalog.
- Search for services.
- Open the Employee Lifecycle Request.
- Submit onboarding or offboarding requests.
- View submitted requests.
- Track request information.
- View request activity and status.

The project includes screenshots documenting the Service Portal and request process.

---

## 6. Request Processing

When a user submits an Employee Lifecycle Request, ServiceNow creates the corresponding request and requested item records.

The request can then progress through the configured lifecycle.

The major processing stages include:

1. Request submission.
2. Request creation.
3. Requested item creation.
4. Approval processing.
5. Workflow or Flow Designer automation.
6. Task creation.
7. Lifecycle task execution.
8. SLA monitoring.
9. Notifications.
10. Request completion.

---

## 7. Approval Process

The application includes an approval stage for employee lifecycle requests.

The request record provides an approval status such as:

- Not Yet Requested
- Requested
- Approved
- Rejected

After the required approval is completed, the request can proceed to the next stage of processing.

The demonstrated application contains an approved employee lifecycle request and corresponding requested item records.

---

## 8. Flow Designer Automation

Flow Designer is used to automate employee lifecycle processing.

The automation is intended to reduce manual processing and provide consistent execution of lifecycle activities.

The automation can perform activities such as:

- Detecting the submitted request.
- Evaluating the request type.
- Processing approval requirements.
- Creating lifecycle tasks.
- Updating request or task states.
- Supporting SLA-related processing.
- Triggering notifications.
- Progressing the request through the employee lifecycle.

---

## 9. Employee Lifecycle Tracking

Employee lifecycle information is maintained through ServiceNow records.

The application supports tracking of:

- Employee name.
- Employee ID.
- Department.
- Manager.
- Request type.
- Request status.
- Approval status.
- Requested item.
- Lifecycle stage.
- Tasks.
- Due dates.
- Additional request information.

This provides a centralized record of the employee lifecycle process.

---

## 10. Request and Requested Item Records

ServiceNow separates the overall request from the individual requested item.

### Request Record

The Request record contains information such as:

- Request number.
- Requested for.
- Opened date.
- Opened by.
- Approval.
- Request state.
- Description.
- Short description.
- Special instructions.
- Work notes.
- Related requested items.

### Requested Item Record

The Requested Item record contains information such as:

- Requested item number.
- Catalog item.
- Request reference.
- Requested for.
- Opened date.
- Stage.
- State.
- Quantity.
- Due date.
- Employee lifecycle variables.

The requested item also displays the variables submitted through the Employee Lifecycle Request catalog item.

---

## 11. Request States

The application uses ServiceNow request state management to represent request progress.

The demonstrated request record supports states including:

- Pending Approval
- Approved
- Closed Complete
- Closed Incomplete
- Closed Cancelled
- Closed Rejected
- Closed Skipped

The appropriate state represents the current processing status of the request.

---

## 12. Lifecycle Stages

The requested item uses lifecycle stages to represent progress through the employee request process.

For example, an approved request can display a stage such as:

**Request Approved**

The stage provides an additional indication of where the requested item is within the lifecycle process.

---

## 13. Task Management

Employee lifecycle processing can generate tasks required to complete onboarding or offboarding activities.

Tasks provide a structured way to assign and track individual lifecycle activities.

Task management supports:

- Task creation.
- Assignment.
- Task state tracking.
- Due dates.
- Completion tracking.
- Relationship with the employee lifecycle request.

---

## 14. SLA Configuration

Service Level Agreement monitoring is included in the application design to support time-based tracking of employee lifecycle activities.

SLA management can be used to monitor:

- Request processing time.
- Task completion time.
- Due dates.
- Processing targets.
- SLA status.

This helps ensure that employee lifecycle activities are completed within the required timeframe.

---

## 15. Notifications

Notifications are used to communicate important lifecycle events.

Potential notification events include:

- Request submission.
- Approval request.
- Approval completion.
- Task assignment.
- Task updates.
- Request completion.
- SLA-related events.

Notifications improve visibility for users, approvers, and teams involved in the lifecycle process.

---

## 16. Role-Based Access

The application supports role-based access to control who can perform specific operations.

Access control can be applied to:

- Employee lifecycle requests.
- Request records.
- Requested items.
- Lifecycle tasks.
- Administrative configuration.
- Application data.

This helps prevent unauthorized users from modifying protected application information.

---

## 17. Service Portal Demonstration

The application was tested through the ServiceNow Service Portal.

The demonstrated process includes:

1. Opening the Service Portal.
2. Accessing the Service Catalog.
3. Searching for the employee lifecycle service.
4. Opening the Employee Lifecycle Request.
5. Selecting the request type.
6. Entering employee information.
7. Submitting the request.
8. Viewing the generated request.
9. Viewing the requested item.
10. Reviewing approval information.
11. Viewing the request status.
12. Viewing the order/request completion information.

---

## 18. Screenshot Evidence

The project contains the following screenshots under the `screenshots` directory:

| No. | Screenshot | Purpose |
|---|---|---|
| 01 | `01-service-portal.png` | ServiceNow Service Portal |
| 02 | `02-service-catalog.png` | Service Catalog interface |
| 03 | `03-employee-lifecycle-request-form.png` | Employee Lifecycle Request form |
| 04 | `04-request-record.png` | ServiceNow request record |
| 05 | `05-approval.png` | Request approval information |
| 06 | `06-requested-item.png` | Requested Item record and lifecycle variables |
| 07 | `07-my-request.png` | User-facing My Request view |
| 08 | `08-approved-request.png` | Approved request state |
| 09 | `09-order-status.png` | Order/request status confirmation |

These screenshots provide visual evidence of the application's user interface and request processing stages.

---

## 19. Testing and Validation

The application was validated through the ServiceNow interface.

The validation process included checking:

- Service Portal access.
- Service Catalog availability.
- Employee Lifecycle Request visibility.
- Required catalog variables.
- Request submission.
- Request record creation.
- Requested Item creation.
- Approval state.
- Request state.
- Requested Item stage.
- Employee lifecycle variables.
- User-facing request information.
- Order status information.

The demonstrated records confirm that employee lifecycle requests can be submitted and represented through ServiceNow request and requested-item records.

---

## 20. Source Control

The application source is maintained using ServiceNow Studio Source Control and GitHub.

The GitHub repository contains the project source and supporting documentation.

The repository includes:

- `docs/`
- `screenshots/`
- `project-report/`
- `update-set/`
- ServiceNow application source files
- `README.md`
- `sn_source_control.properties`

GitHub provides centralized version control and makes the application structure and development history accessible.

---

## 21. Update Set and Development History

Completed update set history was migrated into source control commits to preserve development history.

This provides traceability between ServiceNow configuration changes and Git commits.

The repository therefore provides a historical record of application development and documentation changes.

---

## 22. Deployment Process

The application follows a source-controlled development process.

The general deployment process is:

1. Develop or modify the application in ServiceNow.
2. Test the changes in the development instance.
3. Commit changes using ServiceNow Studio Source Control.
4. Verify the changes in GitHub.
5. Create or update a Pull Request when required.
6. Review the changed files.
7. Merge the Pull Request into the `main` branch.
8. Validate the application after deployment.

---

## 23. Post-Deployment Validation

After deployment or source-control changes, the following areas should be validated:

- Service Catalog items.
- Employee onboarding workflow.
- Employee offboarding workflow.
- Approval process.
- Flow Designer automation.
- Task creation.
- SLA configuration.
- Notifications.
- Role-based access.
- Employee lifecycle records.
- Service Portal functionality.
- Request and Requested Item states.

---

## 24. Version Control Benefits

Using GitHub source control provides:

- Change history.
- Version tracking.
- Collaboration.
- Pull Request workflow.
- Deployment traceability.
- Recovery from previous versions.
- Centralized project management.
- Documentation management.
- Easier review of configuration changes.

---

## 25. Repository Documentation Structure

The project documentation is organized into separate folders to keep the repository maintainable.

### `docs/`

Contains technical documentation such as:

- System architecture.
- Project setup guide.
- Application demonstration guide.
- Testing documentation.
- Deployment and source-control documentation.

### `screenshots/`

Contains visual evidence of the application.

### `project-report/`

Contains the formal project report.

### `update-set/`

Contains update-set-related project artifacts and documentation.

---

## 26. Project Architecture Summary

The overall application architecture can be summarized as:

```text
User
  |
  v
Service Portal
  |
  v
Service Catalog
  |
  v
Employee Lifecycle Request
  |
  v
Request / Requested Item
  |
  v
Approval Process
  |
  v
Flow Designer Automation
  |
  +------------------+
  |                  |
  v                  v
Tasks              Notifications
  |
  v
SLA Monitoring
  |
  v
Employee Lifecycle Completion
