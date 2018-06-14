### Name
- Add Task

### Summary
- New task item adds to the Schedule

### Rationale
- Schedule of sessions should be up-to-date. So the Admin should be able to add, delete or edit the session.

### Users
- Admin

### Preconditions
- The User should have admin rights and stay on the Schedule page

### Basic Course of Events
1. The User indicates that Schedule page has "Add Task" button. 
2. The User clicks that button. 
3. The "New Task" form appears on the page under button block.
4. The User fills the required "Title" field. 
5. The User chooses "required" Task Type from the dropdown list. The possible types:
    - Task 
    - Code Jam 
    - Interview
    - Test
6. The User chooses the start date of the task in the required field "Start Date".
7. The User chooses the start time of the task in the required field "Start Time".
8. The User chooses the end date of the task in the required field "End Date".
9. The User chooses the end time of the task in the required field "End Time".
10. The User chooses the path of the task checking from the "Who checks" dropdown list. This choice should be "required". The task can be checked by:
    - Mentor
    - Random Mentor
    - Trainer
    - Unit Test
    - External Person
    - Without Checking
    - Codewars
    - Codecademy
    - Duolingo
11. The User fills the required "URL to Gist/GitHub Markdown File with task description" field. The User should provide a link to the Gist/GitHub Markdown File with task description.
12. The User clicks the "Save" button to add the task to Schedule. If the form was filled in the right way, see Step 13. In case of wrong filling of some fields, the system shows "valid" or "invalid" feedback under all fields.
13. The "New Task" form hides from the page.

### Alternative Paths
- In steps 4-11, The User can decide not to add the new task to the schedule. In this case, the User clicks the "Cancel" button. Then the "New Task" form hides from the page. 

### Postconditions
In case of the successfully adding task, the added task is shown in the schedule in the special place(s): 
- once, if the task has the same dates of Start and End. 
- twice, if the task has the different dates of Start and End: the first place is according to the Start date & Start time, the second place is according to the End date & End time.
Otherwise, the Schedule is unchanged.

### Prototype 
- https://sonejka.github.io/rs-kittens/dist/admin-schedule.html
