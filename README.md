# The Rolling Scopes School App

### MVP Release Date - 10-SEP-2018

# Overview 
   RSSchool функционирует уже более 5 лет. За последние полтора года количество менторов в одном наборе увеличилось до 90, а студентов до 1000+. При таком количестве студентов и менторов стало сложно организовывать и поддерживать учебный процесс, используя преимущественно Google Spreadsheets.

 ### Какие проблемы предполагается решить в рамках MVP:
   - Нет единого профайла студента. Сложно собрать в один документ: 
       - фидбек по выполненным студентом таскам
       - результаты пройденых студентом интервью 
       - общий фидбек ментора по студенту 
   - Нет единого профайла ментора. Сложно отслеживать:
       - количество студентов на каждом этапе обучения
       - количество проведенных интервью, а также фидбеки, которые писал ментор.
   - Score Spreadsheet очень часто ломается. Его необходимо сделать read-only, с возможностью проставления оценки через систему и последующей репликации оценки в score.
   - Нет единого лога событий (кто что сдал, какие проставились оценки и т.д.)
   
 ### Второстепенные проблемы:   
   - Нет трекинга активности студента. Иногда нет возможности понять, учится студент или уже нет. В прошлом наборе несколько студентов вылетели в результате заминки с менторами и невозможности оперативно отследить ситуацию. 
   - Нет возможности быстрой нотификации участников учебного процесса. Например, при изменении расписания занятий или очередном codejam таске. 
   - Нет интеграции с MSOutlook. Система должна присылать митинг реквесты тренерам. 
   - Нет возможности автоматически раздавать электронные сертификаты об обучении в школе
   - Нет поддержки более одного стримов/бранчей обучения одновременно (2018Q1, 2018Q1 BSU, 2018 BSUIR и тд)
      - Нет возможности эффективно стартовать школу в новой локации (Сейчас за пределами РБ подобная школа есть только в Львове)
      - Нет возможность запускать школу чаще чем 2 раза в год. Создавать отдельные короткие/длинные курсы. Нет возможности индивидуального подхода в обучении.
      - Необходима возможность создания/изменения/удаления стримов.
   - Студентов, которым нужна практика, необходимо сразу привязывать только к ЭПАМ менторам
   - Отчеты о работе менторов - количестве ментии и проведенных интервью
   - Подписать название компании у менторов 
   - Интеграция с GitHub
      - автоматизация выдачи приватных репозиториев cтудентам
      - сохранение в систему результатов ревью PR менторами 
   - Аналитика
      -  Даты и время, когда студенты/менторы последний раз заходили в систему
      
### Группы пользователей в рамках MVP
 - Student
 - Admin. Принадлежность к данной роли на основании конфигурации в репозитории.
 - Mentor. Принадлежность к данной роли на основании Admin аппрува. Лекторы тоже относятся к данной категории. 
      
### Функциональные требования в рамках MVP
   1. Login Page ([Прототип](https://sonejka.github.io/rs-kittens/dist/login.html))
      - Возможность залогиниться как студент или как ментор
      - Все пользователи (менторы и студенты) логинятся только через GitHub
      - Все пользователи автоматически ассайнятся на курс 2018Q3
      - Админ должен аппрувнуть профайл ментора после его заполнения ментором
      - Студенты автоматически ассайнятся в общую группу "без ментора"
      - После логина студенты видят Student View
      - После логина менторы видят Mentor View
   2. Список страниц для Student View
         - Профайл Студента [Прототип](https://sonejka.github.io/rs-kittens/dist/student-profile.html)
         - Таски [Прототип](https://sonejka.github.io/rs-kittens/dist/student-tasks.html)
         - Расписание Read-only [Прототип](https://sonejka.github.io/rs-kittens/dist/schedule.html)
         - Мой ментор [Прототип](https://sonejka.github.io/rs-kittens/dist/student-mentor.html)
   3. Список страниц для Mentor View
         - Профайл Ментора [Прототип](https://sonejka.github.io/rs-kittens/dist/mentor-profile.html)
         - Расписание Read-only [Прототип](https://sonejka.github.io/rs-kittens/dist/schedule.html)
         - TODO лист ментора [Прототип](https://sonejka.github.io/rs-kittens/dist/mentor-todo-list.html)
         - Мои студенты [Прототип](https://sonejka.github.io/rs-kittens/dist/mentor-students.html) 
           - Возможность отчислять студентов, указывая причину
         - Оценка тасков/интервью/презентаций
   4. Admin View
      - Управление расписанием [Прототип](https://sonejka.github.io/rs-kittens/dist/admin-schedule.html)
         - [Требования](/use-cases/ui-description-admin-schedule.md)
      - Управление менторами
         - Возможность аппрувнуть профайл потенциального ментора
         - Возможность приглашать менторов на основании результатов гугл формы "mentors wanted" (csv/excel и т.д.) через инвайты
      - Управление группами Mentor-Student
         - Название группы студентов - Имя и Фамилия Ментора
         - Возможность рандомно распределить студентов по группам 
         - Возможность добавлять/отчислять студентов 
         - Возможность перевести студента в другую группу
      - Управление ассайментами
         - Возможность залить оценки по определенному таску из excel. Формат: github аккаунт студента - оценка - комментарий. Будет использоваться для тестов по html/css, результатов интервью и т.д.  
   5. 404 page - https://sonejka.github.io/rs-kittens/dist/404.html
   6. Репликация оценок в Score (Google Spreadsheet)
   7. Автоматизированная процерка тасков
      - Duolingo (раз в сутки)
      - Lingualeo (раз в сутки)
      - Codewars (раз в сутки до определённой даты)
      - Codeschool (Chrome DevTools, HTML/CSS) (определённая дата)
   
### Нефункциональные требования
   - Стабильная работа на desktop/tablet/mobile
   - Поддержка браузеров последней версии. 
   - Работоспособность системы 24/7 желательна, но не обязательна
   - Нагрузка - до 1200 студентов в одном наборе
   
### Схема данных (Draft)
![data scheme](http://varabei.com/public/RSSchoolApp.png)

#### Комментарии
1. Assignments
   - При создании нового таска, ассаймет для каждого студента курса создаётся автоматически. 
   - Начальный статус - Assigned, далее после выполнения студентов задания - ReadyForReview. Ментор проверяет и либо ставит оценку, либо отправляет на переделку (Rejected или Сhecked).

### Git repositories
- https://github.com/rolling-scopes/rsschool-ui
- https://github.com/rolling-scopes/rsschool-api
- https://github.com/rolling-scopes/rsschool-docs
- https://github.com/rolling-scopes/rsschool-scripts
   
### Prototype
  - https://sonejka.github.io/rs-kittens/dist/
  
# C чего начать?
1. Присоединиться к [slack группе](https://join.slack.com/t/rsschool-app/shared_invite/enQtNDEyOTUyOTUyOTY1LWNhMTUwNjk5ZWY1ODYyMDE4ZDVhM2RhZGU2MDU2MGU1ZTczZjgyZjNiYTgyYzExYTY3MDc5ZWM0Y2NlMzcxZTg)
2. Прочитать CONTRIBUTING.md 
    - [rsschool-ui](https://github.com/rolling-scopes/rsschool-ui/blob/master/CONTRIBUTING.md)
    - [rsschool-api](https://github.com/rolling-scopes/rsschool-api/blob/master/CONTRIBUTING.md)
3. Ознакомиться с циклом статей, посвященных разработке приложения - https://medium.com/rs-school

# Crew
  - [Dzmitry Varabei @dzmitry-varabei](https://github.com/dzmitry-varabei/) - Project Owner
  - [Andrei Palchys @apalchys](https://github.com/apalchys) - Dev Lead
  - [Kseniya Varabei @sonejka](https://github.com/sonejka) - UX & Prototype
  - [Tsikhan Shcharbakou @forkollaider](https://github.com/forkollaider) - Tasks  
  - [Nikita Rudy @NikitaRudy](https://github.com/NikitaRudy) -  User profile
  - [Siarhei Smantsar @SIARHEI-SMANTSAR](https://github.com/SIARHEI-SMANTSAR) - Schedule / Batch update
  - [Yuliya Haluza @yuliaHope](https://github.com/yuliaHope) - Tasks
  - [Miatselski Mikhail @mmetelskiy](https://github.com/mmetelskiy) - Notifications 


 
