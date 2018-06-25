### Page
- Admin Schedule

### Users
- Admin

### Preconditions
- The User should have admin rights and stay on the Schedule page

### Description
- The Schedule page enables the User to add, delete or edit the Schedule items (sessions and tasks). The Schedule is up-to-date as a result.

### Navigation 
- Navigation to the Schedule page is by clicking the "Schedule" link in the navigation area in the upper right page corner.

### Issues

### Elements
- The following is a list of all elements in this Schedule page.

    ##### "Add Session"
    - Type: Button
    - Behaviour: when the User clicks on this button, the "Add Session" pop-up window appears.
    - Comments: see the ["Add Session"](https://github.com/rolling-scopes/rsschool-docs/blob/master/use-cases/add-session.md) use case.
    
    ##### "Add Task"
    - Type: Button
    - Behaviour: when the User clicks on this button, the "Add Task" pop-up window appears.
    - Comments: see the ["Add Task"](https://github.com/rolling-scopes/rsschool-docs/blob/master/use-cases/add-task.md) use case.
    
    ##### "Schedule" Row
     - Type: Button
     - Content:
        - Task/session Type (Task Types can be: "Task", "Code Jam", "Interview", "Test". Session Types can be: "Online", "Offline", "Self-learning", "Extra Event".)
        - Task/session Date
        - Task/session Day
        - Task/session Time
        - Task/session Title
        - Task/session Trainer or Who checks
     - Behaviour:  when the User clicks on this button (looks like a table row), the container with the task/session details expands/collapses.
     
     ##### Expanded container with the task/session details
     - Comment: Container with the task/session details expands after clicking on the "Schedule" Row.
     - Content:
        - Task/session Title
        - Task/session Details
        - Buttons: 
            - "Copy" (see the ["Copy Task or Session"](https://github.com/rolling-scopes/rsschool-docs/blob/master/use-cases/copy-task-or-session.md) use case)
            - "Edit" (see the ["Edit Task or Session"](https://github.com/rolling-scopes/rsschool-docs/blob/master/use-cases/edit-task-or-session.md) use case)
            - "Delete" (see the ["Delete Task or Session"](https://github.com/rolling-scopes/rsschool-docs/blob/master/use-cases/delete-task-or-session.md) use case)
            
### Prototype 
- https://sonejka.github.io/rs-kittens/dist/admin-schedule.html
