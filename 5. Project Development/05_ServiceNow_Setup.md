# 5. Project Development – ServiceNow Setup

## Step 1: Open Flow Designer

In the ServiceNow application navigator:

`All > Process Automation > Flow Designer`

Select **New > Flow**.

## Step 2: Create Flow

Name:

`Auto Ticket Classification - Incident Routing`

Description:

`Automatically classifies new Incident records and routes them to the appropriate support group using Flow Designer keyword rules.`

## Step 3: Configure Trigger

Select:

`Record`

Event:

`Created`

Table:

`Incident [incident]`

Save the trigger.

## Step 4: Add Classification Logic

Add an **If** block.

Use the trigger record's Short description and/or Description.

### Branch A – Access

Keywords:
- password
- login
- account
- access
- locked

Actions:
- Category = appropriate service category
- Subcategory = Login/Access
- Assignment Group = IT Service Desk

### Branch B – Hardware

Keywords:
- laptop
- desktop
- keyboard
- mouse
- printer

Actions:
- Category = Hardware
- Subcategory = appropriate hardware value
- Assignment Group = Hardware Support

### Branch C – Network

Keywords:
- wifi
- wi-fi
- network
- vpn
- internet

Actions:
- Category = Network
- Subcategory = appropriate network value
- Assignment Group = Network Support

### Branch D – Email

Keywords:
- email
- outlook
- mailbox
- mail

Actions:
- Category = appropriate category
- Subcategory = Email
- Assignment Group = Email Support

### Branch E – Software

Keywords:
- software
- application
- install
- installation
- app

Actions:
- Category = Software
- Subcategory = appropriate value
- Assignment Group = Application Support

### ELSE

Assign to:

`Service Desk`

This group should exist in the training instance.

## Step 5: Update Record

Use the **Update Record** action.

Record:

`Trigger → Incident Record`

Set the fields required by your project.

## Step 6: Save and Activate

Save the flow and select **Activate**.

## Step 7: Test

Create a new Incident with each sample description from the testing folder.

## Important

Do not hard-code group sys_ids unless your instructor specifically requires them. Reference the assignment group using the ServiceNow field picker.
