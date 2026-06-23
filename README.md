# ServiceNow Task 1 - Custom Field and Choice Value

## Objective

The objective of this task was to customize the Incident table by creating a new custom field and adding a new category choice value.

### Requirements

1. Create a new Incident field:

   * Label: sFone Model
   * Type: String
   * Length: 40

2. Add a new Incident Category:

   * Label: sFone
   * Value: sfone

3. Verify the configuration by creating an Incident record.

---

## Concepts Covered

* ServiceNow Tables
* Records
* Fields
* Forms
* Dictionary Entries
* Choice Lists
* Form Layout
* sys_dictionary
* sys_choice

---

## Implementation Steps

### Step 1: Open Incident Form

Navigate to:

Incident → Create New

Open a new Incident record.

### Step 2: Configure Form Layout

Right-click the Incident form header.

Select:

Configure → Form Layout

### Step 3: Create Custom Field

Create a new field with:

* Name: sFone Model
* Type: String
* Length: 40

ServiceNow automatically creates:

u_sfone_model

in the Incident table.

### Step 4: Add Field to Form

Move the newly created field from Available Fields to Selected Fields.

Save the form layout.

### Step 5: Add Category Choice

Open Category field configuration.

Add a new choice:

* Label: sFone
* Value: sfone

Save the choice.

### Step 6: Verify

Create a new Incident:

* Caller: Megan Burke
* Category: sFone
* sFone Model: sFone Pro
* Short Description: My sFone will not turn on

Submit the record.

---

## Result

Successfully created:

* Custom field: sFone Model
* Custom category: sFone
* Verification Incident

The Incident was created successfully and appeared in the Incident list.

---

## Tables Used

### incident

Stores Incident records.

### sys_dictionary

Stores field definitions.

### sys_choice

Stores choice values.
