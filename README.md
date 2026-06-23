# ServiceNow Developer Capstone Project

This repository contains my complete ServiceNow Developer Capstone Project implementation performed in a ServiceNow Personal Developer Instance (PDI).

The project is being completed task-by-task with both theoretical understanding and practical implementation.

---

## Project Objectives

- Learn ServiceNow Administration
- Understand ServiceNow Development Concepts
- Gain hands-on experience with ITSM
- Implement real-world business requirements
- Build a professional GitHub portfolio

---

## Tasks Completed

### Task 1 – Custom Field and Choice Value Configuration

#### Objective
Create support for Strawberry Phone (sFone) incidents.

#### Activities Performed

- Created custom Incident field:
  - Label: sFone Model
  - Type: String
  - Length: 40

- Added custom Incident Category:
  - Label: sFone
  - Value: sfone

- Added field to Incident Form Layout

- Created verification Incident

#### Concepts Learned

- Tables
- Records
- Fields
- Dictionary Entries
- Choice Lists
- Form Layout
- sys_dictionary
- sys_choice

#### Verification

Successfully created incident:

- Caller: Megan Burke
- Category: sFone
- sFone Model: sFone Pro

---

### Task 2 – User Administration

#### Objective

Create a dedicated support team for Strawberry Phone incidents.

#### Activities Performed

- Navigated to Service Desk Group
- Created child group:
  - Strawberry Support

- Assigned Group Manager:
  - Fred Luddy

- Added ITIL Role

- Added Members:
  - Beth Anglin
  - Bud Richman
  - David Loo
  - Karla Prince
  - Waldo Edberg

- Updated User Record:
  - Manager of Karla Prince → Fred Luddy

#### Concepts Learned

- Users
- Groups
- Roles
- Group Hierarchy
- Group Membership
- Manager Relationships
- Role-Based Access Control (RBAC)

#### Verification

Successfully verified:

- Strawberry Support Group exists
- Fred Luddy assigned as Manager
- ITIL Role assigned
- Members added successfully

---

## Repository Structure
