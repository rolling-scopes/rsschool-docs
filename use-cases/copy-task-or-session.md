### Name
- Copy a Task/Session

### Summary
- A new Task/Session item is created based on a copy of the existing task/session.

### Rationale
- The Schedule should be up-to-date. So the Admin should be able to add, delete or edit the task/session. 
- To simplify the addition of a new task/session item, the User can copy the existing task/session and, on its basis, create a new task/session by changing some fields.

### Users
- Admin

### Preconditions
- The User should have admin rights and stay on the Schedule page

### Basic Course of Events
1. The User notices that Schedule page has the list of tasks/sessions. 
2. The User clicks the row with the task/session that he/she wants to copy.
3. The User notices that the task/session row is expanded after clicking.
4. The User notices that the expanded task/session row has "Copy" button in the upper right corner.
5. The User clicks the "Copy" button.
6. The User notices the pop-up window with "Copy task"/"Copy session" form.
7. In case of session copying the User can edit fields described in the ["Add Session"](https://github.com/rolling-scopes/rsschool-docs/blob/master/use-cases/add-session.md) (steps 4-10). In case of task copying the User can edit fields described in the ["Add Task"](https://github.com/rolling-scopes/rsschool-docs/blob/master/use-cases/add-task.md) (steps 4-11).
8. The User clicks the "Save" button to save the new task/session to the Schedule. If the form was edited in the right way, see Step 9. In case of wrong filling of some fields, the system shows "valid" or "invalid" feedback under all fields.
9. The "Copy task"/"Copy session" pop-up window hides from the page.

### Alternative Paths
- In step 7, The User can decide not to copy the task/session. The User has some ways to close the pop-up window:
    - click on the "backdrop" of the pop-up window ;
    - click the iconic "X" button in the upper right corner;
    - click the "Cancel" button.
- The pop-up window hides from the page.

### Postconditions
In case of the successfully copying of the task/session item, the new task/session item is shown in the schedule in the special place according to the date and time. Otherwise, the Schedule is unchanged.

### Prototype 
- https://sonejka.github.io/rs-kittens/dist/admin-schedule.html
