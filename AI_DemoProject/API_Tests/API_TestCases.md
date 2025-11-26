# API Test Cases – Reservation System

| ID     | Scenario                          | Test Steps                                                                 | Expected Result                                      |
|--------|-----------------------------------|----------------------------------------------------------------------------|------------------------------------------------------|
| API-001| Get reservation list              | 1. Send GET request to `/reservations`                                     | Response returns list of reservations with correct data |
| API-002| Create a new reservation          | 1. Send POST request to `/reservations` with valid data                    | Response status 201, reservation is created and returned |
| API-003| Create reservation with invalid data | 1. Send POST request to `/reservations` with invalid payload (e.g., missing fields) | Response status 400, error message returned           |
| API-004| Update reservation                | 1. Send PUT request to `/reservations/{id}` with updated data              | Response status 200, reservation data is updated      |
| API-005| Delete reservation                | 1. Send DELETE request to `/reservations/{id}`                             | Response status 200, reservation is removed           |
