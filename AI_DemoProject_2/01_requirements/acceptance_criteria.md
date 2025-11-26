# Acceptance Criteria – ToDo Application

## Story: As a user I want to add a task so that I can manage my work
- AC1: The "Title" field is required (min 3, max 80 characters).
- AC2: "Priority" must be one of {Low, Medium, High}. Default = Medium.
- AC3: After successful creation, the task appears in the list without page reload.
- AC4: API `POST /tasks` returns 201 with JSON {id, title, description, priority, completed:false}.
- AC5: Validation errors return 400 with a clear message for the missing/invalid field.

## Story: As a user I want to mark a task as completed so that I can track progress
- AC1: Clicking the checkbox changes the task status to completed.
- AC2: Completed tasks are visually distinguished (e.g., strikethrough or faded style).
- AC3: API `PATCH /tasks/{id}` returns 200 with updated field `completed:true`.

## Story: As a user I want to filter tasks so that I can focus on specific priorities
- AC1: Filter by priority shows only tasks with the selected value.
- AC2: Reset filter shows all tasks again.
- AC3: API `GET /tasks?priority=High` returns only tasks with priority=High.

## Story: As a user I want to delete tasks so that I can remove unnecessary items
- AC1: Clicking the delete icon removes the task after confirmation.
- AC2: API `DELETE /tasks/{id}` returns 204 and the task no longer appears in subsequent GET requests.
