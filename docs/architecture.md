# System Architecture

## Project

ServiceNow Employee Lifecycle Automation

## Overview

The Employee Lifecycle Automation system is built on ServiceNow to manage employee onboarding and offboarding through a structured and automated lifecycle.

The application uses Service Catalog, dynamic forms, Flow Designer automation, approvals, task management, SLA monitoring, notifications, role-based access control, and lifecycle tracking.

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
Main Components
Service Catalog
Provides the employee lifecycle request entry point.

Users can submit onboarding and offboarding requests through catalog services.

Dynamic Forms
Forms collect the information required to process employee lifecycle requests.

Flow Designer
Automates request processing, approvals, task creation, notifications, and lifecycle activities.

Approval Management
Requests can pass through approval stages before the associated work is performed.

Task Management
Automated tasks are created and assigned to the appropriate users or teams.

SLA Monitoring
Service-level tracking is used to monitor task/request completion within the expected time.

Notifications
Notifications communicate important lifecycle events to employees, managers, and responsible teams.

Role-Based Security
Access controls and roles restrict users to the operations they are authorized to perform.

Lifecycle Tracking
Employee onboarding and offboarding progress can be tracked from request creation through completion.

Technology Platform
ServiceNow

Service Catalog

Flow Designer

ServiceNow Tables

ServiceNow ACLs

Notifications

SLA Management

Source Control

GitHub

Source Control
The ServiceNow application is connected to GitHub through ServiceNow Source Control.

The GitHub repository is used for version control and maintaining the application source history.
