### Name
- Add Session

### Summary
- New session item adds to schedule

### Rationale
- Schedule of sessions should be up-to-date. So the Admin should be able to add, delete or edit the session.

### Users
- Admin

### Preconditions
- User should have admin rights and stay on the Schedule page

### Basic Course of Events
1. The User indicates that Schedule page has "Add Session" button. 
2. The User clicks that button. 
3. The "New Session" form appears on the page under button block.
4. The User fills the required "Title" field. 
5. The User chooses "required" Session Type from dropdown list. The possible types:
    - Online (for online sessions like webinars)
    - Offline (for offline sessions in the defined venue)
    - Self-learning (if students should learn topic themselves)
    - Extra Event (for optional sessions like meetups, confs and etc.)
6. The User chooses date of session in the required field "Date".
7. The User chooses time of session in the required field "Time"
8. The User fills the required "Location" field. The location can be either a link to the webinar or the address of the venue.
9. The User fills the required "Trainer" field.
10. The User fills the not required "URL to Gist/GitHub Markdown File" field. User should provide link to the Gist/GitHub Markdown File with session materials.
11. The User clicks the button "Save" to add Session to Schedule. If the form was filled in the right way, see Step 12. In case of wrong filling of some fields, the system shows "valid" or "invalid" feedback under all fields.
12. The "New Session" form hides from the page.

### Alternative Paths
- In steps 4-10, The User can decide not to add the new session to the schedule. In this case, the User clicks the "Cancel" button. Then the "New Session" form hides from the page. 

### Postconditions
In case of the successful adding session, the added session is shown in the session schedule in the special place according to date and time. Otherwise, the Schedule is unchanged.

### Prototype 
- https://sonejka.github.io/rs-kittens/dist/admin-schedule.html
