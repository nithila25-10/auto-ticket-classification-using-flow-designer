# 8. Project Demonstration Script

## Demo Duration
5–7 minutes

## Step 1 – Introduction
Say:

> "Our project is Auto Ticket Classification using ServiceNow Flow Designer. The goal is to automatically classify new Incident tickets and route them to the correct support team."

## Step 2 – Show the Flow
Open:

`Flow Designer > Auto Ticket Classification - Incident Routing`

Show:
- Trigger
- Conditions
- Update Record actions
- Default branch

## Step 3 – Create Test Incident

Create an Incident with:

**Short description:**
`Office WiFi is not working`

## Step 4 – Submit

After submission, open the Incident and show:
- Category
- Subcategory
- Assignment group

Expected:

`Network Support`

## Step 5 – Show Flow Execution

Open the flow execution details and show that the flow completed successfully.

## Step 6 – Demonstrate Another Case

Create:

`I forgot my password`

Expected:

`IT Service Desk`

## Step 7 – Explain Default Case

Create a ticket that does not match any keyword.

Expected:

`Service Desk`

## Closing

> "The project demonstrates how Flow Designer can automate repetitive ServiceNow administration tasks and provide consistent Incident routing."
