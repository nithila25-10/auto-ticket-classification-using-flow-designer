# Project Report

## Title
Auto Ticket Classification using Flow Designer

## Abstract

This project automates the classification and routing of ServiceNow Incident tickets using Flow Designer. A newly created Incident is evaluated using predefined keyword rules. Based on the detected issue type, the flow updates classification fields and routes the ticket to an appropriate support group.

## Introduction

Service desks handle many different types of incidents. Manual classification can introduce delays and inconsistent routing. ServiceNow Flow Designer provides a low-code method to automate repetitive business processes.

## Objectives

1. Automate Incident classification.
2. Reduce manual ticket triage.
3. Route incidents to relevant support groups.
4. Improve consistency.
5. Demonstrate ServiceNow administration and Flow Designer skills.

## Modules

### Module 1 – Incident Creation
The user creates a ServiceNow Incident.

### Module 2 – Trigger
Flow Designer detects the newly created Incident.

### Module 3 – Classification
The flow evaluates issue keywords.

### Module 4 – Routing
The correct assignment group is selected.

### Module 5 – Update
Incident fields are updated.

### Module 6 – Default Handling
Unmatched issues are routed to Service Desk.

## Advantages

- Easy to configure
- Reduces repetitive manual work
- Consistent routing
- Low-code solution
- Easy to demonstrate
- Rules can be maintained by administrators

## Limitations

- Keyword rules may miss unusual wording.
- Multiple issue types in one ticket may be ambiguous.
- Assignment group names differ between ServiceNow instances.
- The basic version does not use machine learning.
- Priority automation requires organization-specific rules.

## Future Enhancement

- Predictive Intelligence
- NLP-based classification
- Confidence score
- Learning from historical incidents
- Dashboard for classification accuracy
- Auto-suggestion for agents
