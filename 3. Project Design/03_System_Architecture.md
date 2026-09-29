# 3. Project Design

## High-Level Architecture

```text
+-------------------+
|     End User      |
+---------+---------+
          |
          v
+-------------------+
| Create Incident   |
|   in ServiceNow   |
+---------+---------+
          |
          v
+-------------------+
| Flow Designer     |
| Record Created    |
+---------+---------+
          |
          v
+-------------------+
| Read Description  |
+---------+---------+
          |
          v
+-----------------------------+
| Classification Rules        |
| IF / ELSE IF keyword match  |
+------+--------+------+------+
       |        |      | 
       v        v      v
   Access   Hardware Network  ...
       |        |      |
       +--------+------+ 
                |
                v
+-----------------------------+
| Update Incident             |
| Category / Subcategory      |
| Assignment Group            |
+-------------+---------------+
              |
              v
+-----------------------------+
| Service Desk / Support Team |
+-----------------------------+
```

## Flow Components

### Trigger
Record → Created → Incident.

### Data
Use trigger record fields:
- Number
- Short description
- Description
- Category
- Subcategory

### Logic
Use If / Else If branches.

### Action
Use Update Record to modify the Incident.

## Design Principle

Keep the classification rules simple and readable. For a student project, Flow Designer conditions are preferable to unnecessary scripting.

## Suggested Flow Name

`Auto Ticket Classification - Incident Routing`

## Suggested Scope

Use the appropriate application scope available in the ServiceNow training instance.
