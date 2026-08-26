# Update Set Documentation

## 1. Overview

Update Sets are used in ServiceNow to capture configuration changes made during application development.

For the Employee Lifecycle Automation project, update-set-related development changes were maintained as part of the application's development and source-control process.

The project also uses ServiceNow Studio Source Control and GitHub to preserve application source and development history.

---

## 2. Purpose

The purpose of update-set management is to provide a controlled method for tracking ServiceNow configuration changes.

Update Sets can contain configuration changes related to:

* Application configuration
* Service Catalog
* Catalog Items
* Catalog Variables
* Flow Designer configuration
* Business Rules
* Client Scripts
* UI configuration
* Notifications
* Roles and access configuration
* SLA configuration
* Other ServiceNow application components

---

## 3. Employee Lifecycle Automation Changes

The Employee Lifecycle Automation application contains configuration related to employee onboarding and offboarding.

The relevant application configuration includes:

* Employee Lifecycle Request catalog item
* Employee lifecycle variables
* Request processing
* Approval configuration
* Flow Designer automation
* Lifecycle task processing
* SLA-related configuration
* Notifications
* Role-based access
* Service Portal functionality

---

## 4. Development Process

The general development process is:

1. Create or modify configuration in the ServiceNow development instance.
2. Associate the changes with the appropriate development/update process.
3. Test the configuration.
4. Verify the application functionality.
5. Commit application changes through ServiceNow Studio Source Control.
6. Verify the resulting source-control changes in GitHub.
7. Review the changes before deployment.

---

## 5. Source Control Relationship

The project uses GitHub together with ServiceNow Studio Source Control.

The source-control process provides a versioned representation of application configuration and development history.

The repository contains ServiceNow application source files together with supporting documentation.

This provides traceability between ServiceNow development activity and Git commits.

---

## 6. Update Set History

Completed update set history was migrated into source control commits to preserve development history.

This provides traceability between ServiceNow configuration changes and Git commits.

The Git history can therefore be used to review changes made during the development of the Employee Lifecycle Automation application.

---

## 7. Validation Before Deployment

Before deploying configuration changes, the following areas should be validated:

* Service Catalog functionality
* Employee Lifecycle Request
* Request variables
* Onboarding process
* Offboarding process
* Approval processing
* Flow Designer automation
* Task creation
* SLA configuration
* Notifications
* Role-based access
* Employee lifecycle records
* Service Portal functionality

---

## 8. Deployment Considerations

Update-set-related configuration should be tested in the development environment before being promoted to another environment.

The deployment process should include:

1. Review the configuration changes.
2. Validate the application in the development environment.
3. Verify dependencies.
4. Commit the changes to source control.
5. Review the Git changes.
6. Deploy or promote the configuration using the organization's approved ServiceNow process.
7. Validate the application after deployment.

---

## 9. GitHub Repository Structure

Update-set documentation is maintained separately from application source files.

The repository contains:

```text
update-set/
└── update-set.md
