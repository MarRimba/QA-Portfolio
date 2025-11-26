# Test Report – Reservation System

## Summary
- **Application tested:** Reservation System (demo)
- **Test scope:** UI, Backend, API
- **Test period:** November 2025
- **Tester:** Martin Rimbal

## Test Execution Results
| Test ID | Scenario                          | Status | Comments                          |
|---------|-----------------------------------|--------|-----------------------------------|
| UI-001  | User login                        | Pass   | Works as expected                 |
| UI-002  | Login with empty fields           | Fail   | Error message not displayed       |
| UI-003  | Create a new reservation          | Pass   | Reservation saved successfully    |
| UI-004  | Delete an existing reservation    | Pass   | Reservation removed from list     |
| BE-001  | Verify reservation data consistency | Pass | Data matches between UI and backend |
| BE-003  | Invalid reservation input handling | Fail | Backend accepts invalid data      |
| API-002 | Create a new reservation (POST)   | Pass   | Status 201, reservation created   |
| API-003 | Create reservation with invalid data | Fail | Status 200 returned instead of 400 |

## Defects Found
- **BUG-002:** Reservation form allows empty date field  
- **BUG-003:** Deleted reservation still appears in backend response  

## Conclusion
- **Total test cases executed:** 8  
- **Passed:** 5  
- **Failed:** 3  
- **Overall result:** System requires fixes in validation and backend consistency.
