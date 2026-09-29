# Administrator Manual

## Creating Assignment Groups

Create or use appropriate groups in the training instance:

- IT Service Desk
- Hardware Support
- Network Support
- Email Support
- Application Support
- Service Desk

The exact group names may be different in your instance.

## Maintaining Rules

When a new issue type is required:
1. Identify common keywords.
2. Add a new If/Else If branch.
3. Set category/subcategory.
4. Select assignment group from the reference field.
5. Test with at least three sample descriptions.
6. Activate the updated flow.

## Troubleshooting

### Flow did not run
Check:
- Flow is Active.
- Trigger table is Incident.
- Trigger event is Created.
- User has appropriate permissions.

### Assignment group is empty
Check:
- Assignment group exists.
- The flow has permission to update the field.
- The correct reference record is selected.

### Wrong classification
Check:
- Keyword conditions.
- Branch order.
- Multiple keyword matches.
- Default branch.

## Maintenance

Review classification rules periodically and update keywords based on actual support tickets.
