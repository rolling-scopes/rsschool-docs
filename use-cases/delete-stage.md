### Name
- Delete Stage

### Summary
- Stage deletes from the Schedule

### Rationale
- The student learning cycle has to go through some stages. The stages should be up-to-date. So the Admin should be able to add, delete or edit the stages.

### Users
- Admin

### Preconditions
- The User should have admin rights and stay on the Schedule page

### Basic Course of Events
1. The User notices that Schedule page has "Delete" button near the stage title that he/she wants to delete. 
2. The User clicks that button. 
3. a) If the User tries to delete the empty stage, he/she notices the pop-up window with question "Do you really want to delete this stage?" and "Yes"/"No" buttons. Then the User clicks the "Yes" button. 
   b) If the User tries to delete the stage with tasks/sessions, he/she notices the pop-up window with the notification "This Stage cannot be deleted because it is not empty" and "Ok" button. The User clicks the "Ok" button.
4. The pop-up window hides from the page.

### Alternative Paths
- In step 3a, The User can decide not to delete the stage from the schedule. The User has some ways to close the pop-up window:
  - click on the "backdrop" of the pop-up window ;
  - click the iconic "X" button in the upper right corner;
  - click the "No" button.
- The pop-up window hides from the page.

### Postconditions
In case of the successfully deleting stage, the stage hides from the Schedule.
Otherwise, the Schedule is unchanged.

### Prototype 
- https://sonejka.github.io/rs-kittens/dist/admin-schedule.html
