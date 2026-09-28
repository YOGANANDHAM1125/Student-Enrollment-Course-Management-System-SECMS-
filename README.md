# Student Enrollment & Course Management System (SECMS)

## Project Overview

Student Enrollment & Course Management System (SECMS) is a
Salesforce-based project developed using Salesforce Administrator
features and AI Agentforce context.

The system is designed to manage students, courses, instructors,
enrollments, approvals, payments, automation, reports, dashboards, and
security in one centralized Salesforce application.

## Objectives

-   Manage student information
-   Manage course information
-   Manage instructor information
-   Process student enrollments
-   Assign instructors based on course category
-   Automate enrollment-related activities
-   Manage enrollment approval
-   Track fees and revenue
-   Generate reports and dashboards
-   Apply Salesforce security and access controls

## Technology Used

-   Salesforce Lightning UI
-   Salesforce Objects
-   Salesforce Flows
-   Validation Rules
-   Approval Process
-   Reports
-   Dashboards
-   Salesforce Security / Permission Sets
-   AI Agentforce

## Main Salesforce Objects

-   Student
-   Course
-   Instructor
-   Enrollment

### Relationships

The Enrollment object has Lookup Relationships with:

-   Student
-   Course
-   Instructor

## Main Features

### Student Management

Stores student name, email, phone, date of birth, student status, and
address.

### Course Management

Stores course name, category, duration, course fee, and description.

### Instructor Management

Stores instructor name, instructor code, expertise, phone, and email.

### Enrollment Management

Stores student, course, instructor, enrollment date, enrollment status,
fees paid, total amount, and comments.

## Automation

The project contains Salesforce Flows for:

1.  Automatically setting the enrollment date when an enrollment is
    created.
2.  Sending an email and updating student status when an enrollment is
    approved.
3.  Automatically assigning an instructor based on course category.
4.  Creating a follow-up task for requested enrollments.

## Validation Rules

The project contains validation rules for:

-   Student institutional email validation.
-   Preventing an enrollment from being approved before fees are paid.

## Approval Process

An enrollment with status `Requested` can enter the approval process.

The Training Manager is configured as the approver.

After approval, the enrollment status is set to `Approved`.

After rejection, the enrollment status is set to `Rejected` and a
rejection email is sent.

## Reports

The project includes:

-   Students by Status
-   Enrollments by Course
-   Pending Enrollment Approvals
-   Revenue Report -- Fees Paid

## Dashboard

The Student Management Dashboard contains:

-   Students by Status -- Donut Chart
-   Enrollments by Course -- Bar Chart
-   Revenue Report -- Gauge
-   Pending Approvals -- Table

## Security

The project includes security configuration for:

-   Admin -- Full access
-   Enrollment Officer -- Create/Update Enrollments
-   Instructor -- Read-only access to assigned enrollments
-   Permission Sets
-   Organization-Wide Defaults

## Testing

Testing was performed for:

-   Student creation
-   Course creation
-   Instructor creation
-   Enrollment creation
-   Validation rules
-   Record type behavior
-   Flow execution
-   Reports
-   Dashboards

Screenshots are included in the project files.

## Project Files

-   `Project-Document/` -- Complete project documentation PDF
-   `Screenshots/` -- Salesforce configuration and testing screenshots
-   `Salesforce-Configuration/` -- Salesforce object, field, validation,
    flow, approval, report, dashboard, and security details

## Demo

Salesforce Developer Org / Demo Link:

`PASTE-YOUR-SALESFORCE-DEMO-LINK-HERE`

## Skill Wallet

Skill Wallet Project Link:

`PASTE-YOUR-SKILL-WALLET-LINK-HERE`

## Author

**Yoganandham P.**

B.Sc. Computer Science -- III Year

## Conclusion

SECMS provides a centralized Salesforce solution for managing student
enrollment and course-related activities. Salesforce automation,
validation, approval processes, reports, dashboards, and security
features are used to support the complete enrollment management process.
