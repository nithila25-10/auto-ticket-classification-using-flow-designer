# Flow Designer Layout

```text
START
  |
  v
Trigger: Incident Created
  |
  v
Get/Use Trigger Record
  |
  v
IF Access Keywords?
  | YES
  v
Update Incident:
Category = Inquiry / appropriate category
Subcategory = Login/Access
Assignment Group = IT Service Desk
  |
  +---------------- NO ----------------+
                                      |
                                      v
                             IF Hardware Keywords?
                                      |
                           +----------+----------+
                          YES                   NO
                           |                     |
                           v                     v
                    Update Hardware       IF Network Keywords?
                    Support fields              |
                                          +------+------+
                                         YES           NO
                                          |             |
                                          v             v
                                   Update Network   IF Email/Software
                                      Support          Keywords?
                                                        |
                                                        v
                                                  Update respective
                                                     group
                                                        |
                                                        v
                                                ELSE Default Group
                                                        |
                                                        v
                                                       END
```

## Example Condition

Use a condition equivalent to:

`Short description` contains `wifi`

Add related conditions for:
- network
- VPN
- internet

Repeat for each classification branch.

## Note

Field values such as Category, Subcategory and Assignment Group depend on the configuration of the specific ServiceNow instance. Select values from the actual reference fields instead of manually typing record IDs.
