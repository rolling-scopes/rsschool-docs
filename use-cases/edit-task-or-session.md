### Name
- Edit Task/Session

### Summary
- Task/Session edits in the Schedule

### Rationale
- The Schedule should be up-to-date. So the Admin should be able to add, delete or edit the task/session.

### Users
- Admin

### Preconditions
- The User should have admin rights and stay on the Schedule page

### Basic Course of Events
1. The User notices that Schedule page has the list of tasks/sessions. 
2. The User clicks the row with the task/session that he/she wants to edit.
3. The User notices that the task/session row is expanded after clicking.
4. The User notices that the expanded task/session row has "Edit" button in the upper right corner.
5. The User clicks the "Edit" button.
6. The User notices the pop-up window with "Edit task"/"Edit session" form.
7. In case of session editing the User can edit fields described in the ["Add Session"](https://github.com/rolling-scopes/rsschool-docs/blob/master/use-cases/add-session.md) (steps 4-10). In case of task editing the User can edit fields described in the ["Add Task"](https://github.com/rolling-scopes/rsschool-docs/blob/master/use-cases/add-task.md) (steps 4-11).
8. The User clicks the "Save" button to save the changings of task/session to the Schedule. If the form was edited in the right way, see Step 9. In case of wrong filling of some fields, the system shows "valid" or "invalid" feedback under all fields.
9. The "Edit task"/"Edit session" pop-up window hides from the page.

### Alternative Paths
- In step 7, The User can decide not to edit the task/session. The User has some ways to close the pop-up window:
    - click on the "backdrop" of the pop-up window ;
    - click the iconic "X" button in the upper right corner;
    - click the "Cancel" button.
- The pop-up window hides from the page.

### Postconditions
In case of the successfully editing of task/session, the edited task/session changes in the Schedule. Otherwise, the Schedule is unchanged.

### Prototype 
- https://sonejka.github.io/rs-kittens/dist/admin-schedule.html
