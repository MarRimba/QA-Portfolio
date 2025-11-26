# Test Cases – API (ToDo Application)

| ID    | Endpoint       | Method | Input                                      | Expected Result                                                                 |
|-------|----------------|--------|--------------------------------------------|---------------------------------------------------------------------------------|
| API-01 | /tasks         | GET    | -                                          | 200; JSON array; each object has {id:number, title:string[3..80], priority∈{Low,Medium,High}, completed:boolean} |
| API-02 | /tasks         | POST   | {"title":"New Task","priority":"High"}     | 201; response body includes generated id and completed=false                     |
| API-03 | /tasks         | POST   | {"title":""}                               | 400; validation error message for missing title                                  |
| API-04 | /tasks/{id}    | PATCH  | {"completed":true}                         | 200; response body shows completed=true                                          |
| API-05 | /tasks/{id}    | DELETE | -                                          | 204; subsequent GET does not include the deleted task                            |
| API-06 | /tasks         | POST   | {"title":"Valid","priority":"Urgent"}      | 400; validation error for invalid priority value                                 |
