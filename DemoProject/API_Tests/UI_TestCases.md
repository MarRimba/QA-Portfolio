# UI Test Cases – Reservation System

| ID     | Scenario                        | Test Steps                                                                 | Expected Result                                      |
|--------|---------------------------------|----------------------------------------------------------------------------|------------------------------------------------------|
| UI-001 | User login                      | 1. Open the login page<br>2. Enter valid username and password<br>3. Click "Login" | User is redirected to the reservation dashboard      |
| UI-002 | Login with empty fields         | 1. Open the login page<br>2. Click "Login" without entering any data        | Error message appears: "Username and password required" |
| UI-003 | Create a new reservation        | 1. Log in<br>2. Click "Add Reservation"<br>3. Fill in the form<br>4. Click "Save" | Reservation is displayed in the reservation list     |
| UI-004 | Delete an existing reservation  | 1. Log in<br>2. Select an existing reservation<br>3. Click "Delete"         | Reservation is removed from the list                 |