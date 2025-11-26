# Bug Reports – Reservation System

## BUG-001
**Title:** Login button does not respond  
**Steps to Reproduce:**  
1. Open the login page  
2. Enter valid credentials  
3. Click "Login"  
**Expected Result:** User is redirected to the reservation dashboard  
**Actual Result:** Nothing happens, page remains on login screen  
**Status:** Open  
**Severity:** High  

---

## BUG-002
**Title:** Reservation form allows empty date field  
**Steps to Reproduce:**  
1. Log in  
2. Click "Add Reservation"  
3. Leave the date field empty  
4. Click "Save"  
**Expected Result:** Error message appears: "Date is required"  
**Actual Result:** Reservation is saved with empty date  
**Status:** Open  
**Severity:** Medium  

---

## BUG-003
**Title:** Deleted reservation still appears in backend response  
**Steps to Reproduce:**  
1. Log in  
2. Delete an existing reservation  
3. Send GET request to `/reservations`  
**Expected Result:** Deleted reservation is not returned in the response  
**Actual Result:** Reservation still appears in backend response  
**Status:** Open  
**Severity:** High  
