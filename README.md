# Auto Ticket Classification using Flow Designer

## Naan Mudhalvan – ServiceNow Administrator Project

### Project Title
**Auto Ticket Classification using Flow Designer**

### Objective
Automatically classify incoming ServiceNow Incident tickets based on their description/category and route them to the appropriate assignment group. The solution reduces manual triage work and creates a consistent ticket-routing process.

### Main Workflow
1. A new Incident is created.
2. Flow Designer is triggered.
3. The Incident short description and description are evaluated.
4. Matching keywords are identified.
5. Category, subcategory, priority and assignment group are updated.
6. The Incident is saved with the classification result.
7. If no rule matches, the ticket is sent to a default Service Desk group.

### Suggested Technology
- ServiceNow
- Flow Designer
- Incident table (`incident`)
- Flow Designer Trigger
- If / Else If logic
- Update Record action
- Assignment Groups
- ServiceNow Notifications (optional)

### Important
This repository is a project documentation/template package. Flow Designer itself is configured inside a ServiceNow instance, so the included files contain the exact configuration steps, sample data, test cases, scripts and documentation needed to build and demonstrate the project.

## Repository Structure

1. Brainstorming & Ideation
2. Requirement Analysis
3. Project Design
4. Project Planning
5. Project Development
6. Project Testing
7. Project Documentation
8. Project Demonstration

## Quick Build Summary

Create a Flow in:
**All > Flow Designer > New Flow**

Trigger:
**Record created** on **Incident [incident]**

Add classification logic:
- Password / login / account → IT Service Desk / Access Support
- Laptop / desktop / keyboard / mouse → Hardware Support
- Wi-Fi / network / VPN → Network Support
- Email / Outlook / mailbox → Email Support
- Application / software / installation → Application Support
- Otherwise → Service Desk

Then use **Update Record** to update:
- Category
- Subcategory
- Assignment group
- Priority (optional and only according to your organization's rules)

## Expected Result

When a user creates:

> "Unable to connect to office Wi-Fi"

the flow identifies **Network** as the classification and routes the Incident to the configured Network Support assignment group.

