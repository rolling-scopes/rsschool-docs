# Evaluation of assignments

### Data
```
studentId           
assigmentRepo        #string
assigmentComment     #markdown string with predefined template
completeDate
mentorId
mentorComment        #markdown string with predefined template
mentorScore          #number 
checkDate
```

## Возможные сценарии оценки заданий.

### Оценка тасков типа "CodeJam"
```
[Student] Указывает ссылку на репозиторий
[Student] Указывает ссылку на демо страницу
[Student] Оставляет комментарий к работе
[Mentor]  Оставляет комментарий к работе
[Mentor]  Выставляет оценку
```
### Оценка тасков типа "Final Game"
```
[Random Mentor]  Указывает время/место, где он может проверить таски
[Random Student] Апплаится на удобное ему время/место
[Student] Указывает ссылку на репозиторий
[Student] Указывает ссылку на демо страницу
[Student] Оставляет комментарий к работе
[Mentor]  Оставляет комментарий к работе
[Mentor]  Выставляет оценку
```
### Оценка тасков типа "Учебное интервью"
```
[Random Mentor]  Указывает время/место, где он может провести интервью
[Random Student] Апплаится на удобное ему время/место
[Mentor]  Оставляет фидбек по интервью
[Mentor]  Выставляет оценку
```
### Оценка тасков типа "JS Test"
```
[Random Mentor]  Указывает время/место, где он может провести интервью
[Random Student #1] Апплаится на удобное ему время/место
[Random Student #2] Апплаится на удобное ему время/место
....
[Random Student #10] Апплаится на удобное ему время/место
[Random Student #11] Апплаится на удобное ему время/место
[Mentor]  Оставляет фидбек по интервью
[Mentor]  Выставляет оценку
....
[Mentor]  Оставляет фидбек по интервью
[Mentor]  Выставляет оценку
```
