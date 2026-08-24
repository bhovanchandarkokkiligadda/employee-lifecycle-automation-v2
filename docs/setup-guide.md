# Setup Guide

## Prerequisites

- ServiceNow Personal Developer Instance (PDI)
- Access to ServiceNow Studio
- GitHub account
- GitHub repository
- ServiceNow Source Control access

## Application Setup

1. Open the ServiceNow Personal Developer Instance.
2. Open the application in ServiceNow Studio.
3. Verify that the application scope is set to the Employee Lifecycle Automation application.
4. Verify the application components including tables, forms, flows, notifications, roles, ACLs, modules, and catalog configuration.

## Source Control Setup

The application is connected to GitHub using ServiceNow Source Control.

The repository contains the ServiceNow application source and supporting project documentation.

## GitHub Repository

Repository:

`employee-lifecycle-automation-v2`

The main branch is used as the primary project branch.

## Application Verification

Before demonstrating the application, verify:

- Service Catalog is available.
- HR services are accessible.
- Onboarding request can be submitted.
- Offboarding request can be submitted.
- Approval flow is working.
- Tasks are generated.
- Notifications are triggered.
- SLA information is available.
- Requests can reach completion.
- Employee lifecycle information can be tracked.

## Demo Preparation

For the project demonstration, prepare a test employee/request and walk through the complete lifecycle:

Service Catalog → HR Services → Onboard/Offboard Employee → Request Submission → Approval → Task Creation → SLA Monitoring → Notifications → Completion.

## Source Control Verification

After application changes are completed:

1. Commit the changes from ServiceNow Studio.
2. Verify the commit in GitHub.
3. Confirm the changes are present on the appropriate branch.
4. Use the `main` branch as the primary repository view.

## Important

Do not expose passwords, GitHub personal access tokens, API keys, or other credentials in the repository.
