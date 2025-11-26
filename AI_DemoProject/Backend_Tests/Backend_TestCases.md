# Backend Test Cases – Reservation System

| ID     | Scenario                                | Test Steps                                                                 | Expected Result                                      |
|--------|-----------------------------------------|----------------------------------------------------------------------------|------------------------------------------------------|
| BE-001 | Verify reservation data consistency     | 1. Log in<br>2. Create a new reservation<br>3. Check reservation details in the UI<br>4. Inspect backend response (API/Database) | Data in UI matches backend response                  |
| BE-002 | Validate reservation deletion           | 1. Log in<br>2. Delete an existing reservation<br>3. Inspect backend response (API/Database) | Reservation record is removed from backend           |
| BE-003 | Check invalid reservation input handling| 1. Send invalid reservation data (e.g., negative date, empty fields)<br>2. Inspect backend response | Backend rejects invalid data with proper error message |
| BE-004 | Verify reservation list retrieval       | 1. Log in<br>2. Request reservation list from backend<br>3. Compare with UI list | UI list matches backend reservation data             |