# 1. Brainstorming & Ideation

## Problem Statement

In a ServiceNow environment, support teams may receive a large number of Incident tickets every day. Manually reading every ticket and selecting the correct category, subcategory and assignment group takes time and can cause inconsistent routing.

The proposed solution is an **Auto Ticket Classification using Flow Designer** system that automatically analyzes incident information and assigns a suitable classification and support group.

## Existing Problem

- Tickets are manually classified.
- Similar incidents may be assigned differently.
- Manual triage increases response time.
- New support staff may not know the correct assignment group.
- Unclassified tickets can remain in the Service Desk queue.

## Proposed Solution

Build a ServiceNow Flow Designer flow that:
- Starts when an Incident is created.
- Reads the ticket's short description/description.
- Checks predefined keywords.
- Classifies the ticket.
- Updates the Incident.
- Routes it to the correct assignment group.
- Uses a default group when no keyword matches.

## Sample Classification Matrix

| Keywords | Classification | Example Group |
|---|---|---|
| password, login, account, access | Access | IT Service Desk |
| laptop, desktop, keyboard, mouse | Hardware | Hardware Support |
| wifi, network, vpn, internet | Network | Network Support |
| email, outlook, mailbox | Email | Email Support |
| software, application, install | Software | Application Support |

## Scope

### Included
- Incident classification
- Keyword-based routing
- Assignment group update
- Category/subcategory update
- Default routing
- Testing and documentation

### Optional Future Scope
- AI/ML classification
- Natural language processing
- Predictive Intelligence
- Confidence score
- Automatic priority recommendation
- Analytics dashboard

## Innovation

The project demonstrates how low-code/no-code Flow Designer automation can reduce repetitive ticket-triage work without requiring a custom application.
