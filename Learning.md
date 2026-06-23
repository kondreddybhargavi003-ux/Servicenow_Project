# What I Learned

This document contains my learning journey while completing the ServiceNow Developer Capstone Project.

---
# Task 1 – Custom Field and Choice Configuration
## Business Requirement
The organization introduced a new device called Strawberry Phone (sFone).

Service Desk agents need:

- A new category called sFone
- A field to store phone model information

---

## Concepts Learned

### Table

A table stores records.

Examples:

- incident
- task
- sys_user

---

### Record

A single row inside a table.

Example:

INC0010007

---

### Field

A column inside a table.

Examples:

- Caller
- Category
- State

---

### Dictionary Entry

Defines a field's properties.

Stored in:

sys_dictionary

Contains:

- Label
- Type
- Length
- Default values

---

### Choice Field

A dropdown field with predefined values.

Examples:

- State
- Category
- Priority

Choices stored in:

sys_choice

---

### Form Layout

Controls:

- Which fields appear
- Order of fields

---

### Practical Skills Learned

- Create custom field
- Configure form layout
- Add field to form
- Configure choices
- Verify incident creation

---

### Behind the Scenes

Creating a field creates:

- Database Column
- Dictionary Entry

Creating a choice creates:

- sys_choice record

---

# Task 2 – User Administration

## Business Requirement

Create a support team dedicated to Strawberry Phone incidents.

---

## Concepts Learned

### User

Represents a person in ServiceNow.

Stored in:

sys_user

Examples:

- Fred Luddy
- Beth Anglin

---

### Group

Collection of users.

Stored in:

sys_user_group

Examples:

- Service Desk
- Strawberry Support

---

### Role

Defines permissions.

Stored in:

sys_user_role

Examples:

- itil
- admin

---

### Group Membership

Connects users to groups.

Stored in:

sys_user_grmember

---

### Group Manager

Responsible for managing group activities.

Example:

Fred Luddy

Manager of:

Strawberry Support

---

### Role-Based Access Control (RBAC)

ServiceNow security model.

Access is controlled using:

Users → Groups → Roles

---

## Practical Skills Learned

### Create Group

Created:

Strawberry Support

Under:

Service Desk

---

### Assign Group Manager

Assigned:

Fred Luddy

as Group Manager

---

### Assign Role

Added:

itil

role

to the group

---

### Add Members

Added:

- Beth Anglin
- Bud Richman
- David Loo
- Karla Prince
- Waldo Edberg

---

### Update User Record

Updated:

Karla Prince

Manager:

Fred Luddy

---

## Interview Questions Learned

### What is a User?

A person who can log into ServiceNow.

---

### What is a Group?

A collection of users with similar responsibilities.

---

### What is a Role?

A set of permissions assigned to users or groups.

---

### What is RBAC?

Role-Based Access Control.

Used to control access to applications and records.

---

### Difference Between User and Group?

User:
Individual person.

Group:
Collection of users.

---

### Difference Between Group and Role?

Group:
Used for assignment and organization.

Role:
Used for permissions and security.

---

# Overall Learning So Far

I can now:

✅ Create custom fields

✅ Configure choice values

✅ Modify forms

✅ Understand dictionary entries

✅ Understand sys_choice

✅ Create users and groups

✅ Manage group membership

✅ Assign roles

✅ Configure managers
