# Deployment & Source Control

## Overview

The ServiceNow Employee Lifecycle Automation application is maintained using ServiceNow Studio Source Control and GitHub.

The project is connected to a GitHub repository for version control, source tracking, and deployment management.

## Source Control Repository

- **Repository:** `employee-lifecycle-automation-v2`
- **Platform:** GitHub

The ServiceNow application is connected to the repository through ServiceNow Studio Source Control.

## Branch Strategy

The repository uses:

- `main` — primary project branch
- `sn_instances/dev392432` — ServiceNow development instance branch

Changes developed in the ServiceNow instance are committed to the instance branch and can be merged into the main branch through a Pull Request.

## Source Control Workflow

```mermaid
graph TD
    A[ServiceNow Development] --> B[Application Changes]
    B --> C[ServiceNow Source Control Commit]
    C --> D[GitHub Instance Branch]
    D --> E[Pull Request]
    E --> F[Code Review / Validation]
    F --> G[Merge into main]
