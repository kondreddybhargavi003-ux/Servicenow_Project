# ServiceNow Developer Capstone Project

## Project Overview
This repository contains my ServiceNow Developer Capstone Project implementation completed in a Personal Developer Instance (PDI).

The project demonstrates core ServiceNow administration and development concepts including:

- Custom Table Configuration
- Form Customization
- Choice List Management
- User Administration
- Role-Based Access Control (RBAC)
- Service Catalog Management
- Flow Designer Automation
- Catalog Task Fulfillment

---

# Task 1: Custom Field and Choice Value Configuration

## Objective
Enhance the Incident Management process by creating a custom field and a custom choice value.

## Implementation

### Created Custom Incident Field
- Field Name: sFone Model
- Type: String
- Length: 40

### Added New Category Choice
- Choice Label: sFone
- Choice Value: sfone

### Form Customization
- Added sFone Model field to Incident Form Layout.
- Added sFone category to Incident Category choices.

### Verification
- Created a test incident.
- Verified:
  - sFone category appears.
  - sFone Model field is displayed.
  - Incident record saves successfully.

## Concepts Learned
- Tables
- Fields
- Dictionary Entries
- Choice Lists
- Form Layout Configuration
- Metadata Management

---

# Task 2: User Administration

## Objective
Create a support team responsible for handling Strawberry sFone requests.

## Implementation

### Group Creation
Created:

- Strawberry Support

Child Group of:

- Service Desk

### Role Assignment
Assigned:

- itil role

### Group Manager
Assigned:

- Fred Luddy

### Added Members

- Beth Anglin
- Bud Richman
- David Loo
- Kara Prince
- Waldo Edberg

### User Management
Updated Kara Prince record and assigned:

- Manager = Fred Luddy

### Verification
Verified:

- Group created successfully.
- itil role assigned.
- Members added.
- Manager relationship configured.

## Concepts Learned
- Users
- Groups
- Roles
- Role-Based Access Control (RBAC)
- User Hierarchy
- Group Membership Management

---

# Task 3: Automate Service Catalog Item Fulfillment

## Objective
Automate Strawberry sFone request fulfillment using Flow Designer.

## Service Catalog Item
- Strawberry sFone
- Category: Mobiles

## Workflow Name
- Strawberry Workflow

## Flow Design

### Trigger
Catalog Item Requested

### Approval
Requester's Manager Approval

### Approved Path

Catalog Task 1
- Order Strawberry sFone
- Assignment Group: Procurement

Catalog Task 2
- Configure Strawberry sFone
- Assignment Group: Software

Catalog Task 3
- Deliver Strawberry sFone
- Assignment Group: Service Desk

### Completion
Requested Item updated to:

- Closed Complete

### Rejected Path
- Send Rejection Email
- End Workflow

## Verification

### Test Execution
- Ordered Strawberry sFone
- Approved request
- Completed all catalog tasks
- Verified flow execution

### Results
- Tasks created automatically.
- Approval workflow executed successfully.
- Request completed automatically.

## Concepts Learned
- Service Catalog
- Catalog Items
- Requests (REQ)
- Requested Items (RITM)
- Catalog Tasks (SCTASK)
- Flow Designer
- Approvals
- Workflow Automation
- Fulfillment Process

---

# Technologies Used

- ServiceNow Platform
- Incident Management
- User Administration
- Service Catalog
- Flow Designer
- Workflow Automation

---

# Repository Structure

```text
Servicenow_Project/
│
├── Infographic/
│   ├── Task_1.png
│   ├── Task_2.png
│   └── Task_3.png
│
├── Task_1/
│   └── Screenshots/
│
├── Task_2_User_administration/
│   └── Screenshots/
│
├── Task_3_Service_Catalog_Automation/
│   └── Screenshots/
│
├── README.md
└── Learning.md
