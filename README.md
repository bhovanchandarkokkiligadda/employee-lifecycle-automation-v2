# ServiceNow Employee Lifecycle Automation

An Employee Onboarding & Offboarding System built on ServiceNow using Service Catalog, dynamic forms, Flow Designer automation, approvals, employee lifecycle tracking, task management, SLA monitoring, role-based security, notifications, and audit-ready workflow management.

---

## Project Overview

The Employee Lifecycle Automation application provides a centralized ServiceNow solution for managing employee onboarding and offboarding requests.

Users can submit an Employee Lifecycle Request through the Service Portal. The request captures employee information and progresses through the configured approval, automation, task, SLA, and lifecycle management processes.

The project also uses ServiceNow Studio Source Control with GitHub for version control and development traceability.

---

## Key Features

- Employee onboarding request management
- Employee offboarding request management
- Service Catalog integration
- Service Portal access
- Dynamic request forms
- Employee information capture
- Approval processing
- Flow Designer automation
- Requested Item management
- Lifecycle stage tracking
- Task management
- SLA monitoring
- Notifications
- Role-based access control
- Request status tracking
- GitHub source control
- Development history and traceability

---

## Application Flow

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
Approval
  |
  v
Flow Designer Automation
  |
  +------------------+
  |                  |
  v                  v
Tasks            Notifications
  |
  v
SLA Monitoring
  |
  v
Employee Lifecycle Completion
