# Student Tasks Stage1 

### Dev Team
Lead:
Yuliya Haluza @yuliaHope	Skype: yuliaka71, Telegram: @yuliaka71 

Devs:
1) @Zhukovets @nikkaktus24
2) @ymartsevich @grapeperson
3) @anastminsk @VladSanko
4) @Catrieona @mrsDandelion
5) @KurnosovNikita @morzh1205

### Description
На протяжении RSSchool stage#1 студенты решают ряд алгоритмических задач. 
В рамках этого таска необходимо реализовать front-end для сдачи этих задач, а также выполнить интеграцию с созданием тасков на странице [Admin Schedule](https://sonejka.github.io/rs-kittens/dist/admin-schedule.html) 

### Use case
1. Пользователь с ролью `Admin` открывает страницу [Admin Schedule](https://sonejka.github.io/rs-kittens/dist/admin-schedule.html) (Имплементацию делал Siarhei Smantsar @SIARHEI-SMANTSAR Skype: ssi-20). 
2. Создает таск указывая следующие критерии:
   - Task Title: Love triangle
   - Task type: task
   - Start date: 10-SEP-2018 19:00
   - End date: 1-OCT-2018 23:59:00
   - Who checks: Unit test
   - URL: https://github.com/yankouskia/love-triangle
3. Таск добавляется в schedule. На back-end данные по таску хранятся в коллекции 'tasks', каждый студент курса получает новый assignment (коллекция `assignment`)
4. Assignment появляется на странице Student View > Tasks ([Прототип интерфейса](https://sonejka.github.io/rs-kittens/dist/student-tasks.html))
5. Студенты видят:
    - название таска "Love triangle" 
    - ссылку на описание https://github.com/yankouskia/love-triangle
    - поле для выбора репозитория в котором залито их решение задачи
    - поле для комментария
    - кнопку Submit
 6. После нажатия на кнопку submit, заголовок меняет цвет и появляется оценка. 
     Зеленый цвет - 100 баллов (и больше). 
     Желтый цвет - если оценка меньше 100.  
     
### Алгоритм оценки выполненного задания по средствам юнит тестов реализовывать не надо! В рамках задания достаточно показывать рандомную оценку.



