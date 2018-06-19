### Name
- Delete Task/Session

### Summary
- Task/Session item deletes from the Schedule

### Rationale
- Schedule of sessions should be up-to-date. So the Admin should be able to add, delete or edit the task/session.

### Users
- Admin

### Preconditions
- The User should have admin rights and stay on the Schedule page

### Basic Course of Events
1. The User notices that Schedule page has the list of tasks/sessions. 
2. The User clicks the row with the task/session that he/she wants to delete.
3. The User notices that the task/session row is expanded after clicking.
4. The User notices that the expanded task/session row has "Delete" button in the upper right corner.
5. The User clicks the "Delete" button.
6. The User notices pop-up window with question "Do you really want to delete this task/session?" and "Yes"/"No" buttons.
7. The User clicks the "Yes" button.
8. The pop-up window hides from the page.

### Alternative Paths
- In step 7, The User can decide not to delete the task/session from the schedule. The User has some ways to close the pop-up window:
  - click on the "backdrop" of the pop-up window ;
  - click the iconic "X" button in the upper right corner;
  - click the "No" button.
- The pop-up window hides from the page.

### Postconditions
In case of the successfully deleting task/session, the task/session hides from the Schedule.
Otherwise, the Schedule is unchanged.

### Prototype 
- https://sonejka.github.io/rs-kittens/dist/admin-schedule.html
