### Name
- Edit Stage

### Summary
- Stage edits in the Schedule

### Rationale
- The student learning cycle has to go through some stages. The stages should be up-to-date. So the Admin should be able to add, delete or edit the stages.

### Users
- Admin

### Preconditions
- The User should have admin rights and stay on the Schedule page

### Basic Course of Events
1. The User notices that Schedule page has "Edit" button near the stage title that he/she wants to edit.
2. The User clicks that button. 
3. The "Edit Stage" form appears in the pop-up window.
4. The User can edit fields described in the ["Add Stage"](https://github.com/rolling-scopes/rsschool-docs/blob/master/use-cases/add-stage.md) (steps 4-6)
5. The User clicks the "Save" button to add stage to the Schedule. If the form was filled in the right way, see Step 6. In case of wrong filling of some fields, the system shows "valid" or "invalid" feedback under all fields.
6. The "Edit Stage" pop-up window hides from the page.

### Alternative Paths
- In steps 4, The User can decide not to edit the stage. The User has some ways to close the pop-up window:
    - click on the "backdrop" of the pop-up window ;
    - click the iconic "X" button in the upper right corner;
    - click the "Cancel" button. 
- Then the "Edit Stage" pop-up window hides from the page. 

### Postconditions
In case of the successfully editing stage, the edited stage changes in the Schedule. Otherwise, the Schedule is unchanged.

### Prototype 
- https://sonejka.github.io/rs-kittens/dist/admin-schedule.html
