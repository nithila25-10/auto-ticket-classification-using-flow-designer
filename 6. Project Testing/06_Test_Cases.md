# 6. Project Testing

## Test Case Format

| ID | Input | Expected Result | Status |
|---|---|---|---|
| TC01 | I forgot my password | Access → IT Service Desk | Pass/Fail |
| TC02 | Laptop is not turning on | Hardware → Hardware Support | Pass/Fail |
| TC03 | Office WiFi is not working | Network → Network Support | Pass/Fail |
| TC04 | Outlook is not receiving mail | Email → Email Support | Pass/Fail |
| TC05 | Need software installation | Software → Application Support | Pass/Fail |
| TC06 | Random unmatched issue | Default → Service Desk | Pass/Fail |

## Detailed Tests

### TC01 – Password
Input:
`I forgot my password`

Expected:
- Access classification
- Login/Access subcategory
- IT Service Desk assignment

### TC02 – Hardware
Input:
`Laptop is not turning on`

Expected:
- Hardware classification
- Hardware-related subcategory
- Hardware Support assignment

### TC03 – Network
Input:
`Office WiFi is not working`

Expected:
- Network classification
- Connectivity subcategory
- Network Support assignment

### TC04 – Email
Input:
`Outlook is not receiving mail`

Expected:
- Email classification
- Email subcategory
- Email Support assignment

### TC05 – Software
Input:
`I need software installation`

Expected:
- Software classification
- Application subcategory
- Application Support assignment

### TC06 – No Match
Input:
`I have a problem with something else`

Expected:
- Default classification
- Service Desk assignment

## Testing Checklist

- [ ] Flow is activated.
- [ ] Trigger fires on Incident creation.
- [ ] Each branch executes correctly.
- [ ] Incident fields are updated.
- [ ] Assignment group is correct.
- [ ] Default branch works.
- [ ] Flow execution details show success.
