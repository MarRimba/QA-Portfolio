# Test Cases – UI (ToDo Application)

| ID   | Title                     | Steps                                                                 | Expected Result                                      | Priority |
|------|---------------------------|----------------------------------------------------------------------|------------------------------------------------------|----------|
| UI-01 | Add task successfully     | 1. Open app 2. Enter "Refactor report" 3. Select priority=High 4. Save | Task appears in list; toast "Task added"             | High     |
| UI-02 | Empty title validation    | 1. Open app 2. Leave title empty 3. Save                              | Error message near field; task not added             | High     |
| UI-03 | Title length >80 chars    | 1. Enter 81 characters in title 2. Save                               | Validation error: "Maximum 80 characters allowed"    | Medium   |
| UI-04 | Filter by High priority   | 1. Set filter=High                                                    | List shows only tasks with High priority             | Medium   |
| UI-05 | Mark task as completed    | 1. Click checkbox on a task                                           | Task marked completed; style changes (strikethrough) | Medium   |
| UI-06 | Delete task               | 1. Click delete icon 2. Confirm                                       | Task removed; toast "Task deleted"                   | High     |
