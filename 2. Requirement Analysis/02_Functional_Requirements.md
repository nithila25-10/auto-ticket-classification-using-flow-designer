# 2. Requirement Analysis

## Functional Requirements

### FR-01: Incident Trigger
The system shall start the flow when a new Incident record is created.

### FR-02: Read Ticket Text
The flow shall read the Incident short description and/or description.

### FR-03: Keyword Classification
The flow shall compare the ticket text against predefined classification keywords.

### FR-04: Update Classification
The flow shall update the Incident category and subcategory where appropriate.

### FR-05: Assignment
The flow shall set the appropriate assignment group.

### FR-06: Default Routing
If no rule matches, the flow shall assign the ticket to the default Service Desk group.

### FR-07: Traceability
The flow execution shall be visible in Flow Designer execution details.

## Non-Functional Requirements

- Easy to maintain
- Low-code implementation
- Fast execution
- Consistent routing
- Simple demonstration
- Clear documentation
- Minimal custom scripting

## Actors

1. End User – creates an Incident.
2. Service Desk Agent – receives and works on classified tickets.
3. Administrator – maintains the Flow and classification rules.

## Inputs

- Short description
- Description
- Category
- Subcategory
- Caller information

## Outputs

- Classification
- Category
- Subcategory
- Assignment group
- Optional priority

## Assumptions

- Incident table is available.
- Required assignment groups exist or are created in the instance.
- The administrator has permission to create and activate flows.
