# Bug Reports – ToDo Application

## DEF-001 – Double-click on "Save" creates duplicate tasks
- **Severity:** Major  
- **Priority:** High  
- **Environment:** Chrome 129, Windows 11  
- **Steps to Reproduce:**  
  1. Enter title "Duplicate Test".  
  2. Quickly double-click the "Save" button.  
- **Actual Result:** Two identical tasks are created.  
- **Expected Result:** Only one task should be created; second click ignored or blocked.  
- **Evidence:** Screenshot in /06_defects/screenshots/def-001.png  
- **Suggestion:** Disable button after first click or validate idempotency on backend.

---

## DEF-002 – Error message not user-friendly
- **Severity:** Minor  
- **Priority:** Medium  
- **Environment:** Firefox 131, Windows 11  
- **Steps to Reproduce:**  
  1. Leave the "Title" field empty.  
  2. Click "Save".  
- **Actual Result:** Error message shows "400 Bad Request".  
- **Expected Result:** Clear message like "Title is required".  
- **Evidence:** Screenshot in /06_defects/screenshots/def-002.png  
- **Suggestion:** Improve error messages to be understandable for end users.
