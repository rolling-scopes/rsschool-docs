# rsschool-docs

### RSSchool MVP

### Owners
  -  Tsikhan Shcharbakou / Nikita Rudy (Task creation / Tasks review / Task automated checking)

### Users:
  - Students  
  - Mentors
  - Admins

### Students
  - Schedule (read-only). 
      1) Возможность оставить фидбек по отдельно взятой лекции. В рамках MVP фидбек будет сохраняться в гугл форму c pre-filled полем (Например, https://docs.google.com/forms/d/e/1FAIpQLSfEu_DBwq2YN3VuHpEvgIT6FuS5pb9fFGH3MGshbKECJibvKQ/viewform?usp=pp_url&entry.683149895=JavaScript+Intro).
  - Tasks
    - В #stage1 студенты решают алгоритмические таски в своём public репозитории. Сдача таска через выбор public репозитория в интерфейсе системы. Это функциональность есть в https://epa.ms/padawans-2018
    - В #stage2-3 в private репозиторий. Без автоматической проверки. Когда таск готов, студент нажимает кнопку "Ready for review". Оценку ставит ментор.
   - Profile ([как в прототипе](https://sonejka.github.io/rs-kittens/dist/student-profile.html))
   - Your mentor ([как в прототипе](https://sonejka.github.io/rs-kittens/dist/student-mentor.html))
   
    
### Mentors
  - Profile ([как в прототипе](https://sonejka.github.io/rs-kittens/dist/mentor-profile.html))
  - Могут выставлять оценки своим студентам по таскам/презентациям. комментарии к оценкам? **(TBD)**
  - Могут отчислять студентов, указывая причину
  - Могут выдавать темы презентаций
  - Могут записывать результаты интервью
  - 
  
### Admins
 - Может создовать менторов на основании гугл формы (csv/excel и т.д.)
 - Система должна высласть инвайты менторам нового набора **(TBD)**
 - Может создавать занятия (aka  sessions) и таски
 - Возможность выгрузить общий score со всеми оценками в excel. 
 - Возможность перевести студента к другому ментору. (Добавлять/удалять студентов у менторов в ручную)
 - Возможность отчислить студента
 - Возможность просмотреть профайлы менторов и студентов
 - Аналитика 
    - Даты и время, когда студенты/менторы последний раз заходили в систему
 - Возможность залить оценки по определенному таску из excel. Формат: github аккаунт студента - оценка. Будет использоваться для тестов по html/css и т.д.  
 
