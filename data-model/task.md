### Data
```
title                  #string
type                   #enum - Task / CodeJam / Interview / Test
startDate
startTime
endDate
endTime
whoCheck                #enum - mentor / randomMentor / trainer / unit test / externalPerson / withoutChecking / codewars / codeacademy / duolinguo
urlToDescription        # description should be in markdown
studentCommentTemplate  # 
mentorCommentTemplate   #
```

### Use Case
https://github.com/rolling-scopes/rsschool-docs/blob/master/use-cases/add-task.md

### WIP
```
Task
    - title
    - type
    - description
    - due date
    - author
    - mentorTempalte
    - studentTemplate


Assignments
 - task Id
 - mentor Id
 - students Id
 - score

assignTasks(tasks) {
    tasks.map(createAssignment).forEach(createEmailJob)
}
```
