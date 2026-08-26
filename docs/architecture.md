# System Architecture

## Project

ServiceNow Employee Lifecycle Automation

## Overview

The Employee Lifecycle Automation system is built on ServiceNow to manage employee onboarding and offboarding through a structured and automated lifecycle.

The application uses Service Catalog, dynamic forms, Flow Designer automation, approvals, task management, SLA monitoring, notifications, role-based access control, and lifecycle tracking.

---

## Architecture Flow

```mermaid
graph TD
    A[Employee] --> B[Service Catalog]
    B --> C[Onboarding / Offboarding Request]
    C --> D[Dynamic Form]
    D --> E[Request Creation]
    E --> F[Approval Workflow]
    F --> G[Automated Task Creation]
    G --> H[Task Assignment]
    H --> I[SLA Monitoring]
    I --> J[Notifications]
    J --> K[Request Completion]
    K --> L[Lifecycle Tracking]
