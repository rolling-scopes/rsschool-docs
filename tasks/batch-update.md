# Batch update 

### Dev Team
Lead:
Siarhei Smantsar @SIARHEI-SMANTSAR Skype: ssi-20 

Devs:
1) @kakoc @KatieVo
2) @Morfinbrood @LipinArts
3) @YuliyaHlukhatarenka  
4) @Leamhein
5) @NSpeko

### Description
Необходимо реализовать логику по импорту оценок и результатов интервью в RSSchoolApp из xlsx формата.

### Use case
1. Пользователь с ролью `Admin` открывает страницу `Batch update`.
2. В dropdown выбирает курс для которого будет произведен импорт оценок. В рамках MVP есть возможность выбрать только `stream2018Q3`.
3. В dropdown выбирает таск (например `JSCore Interview`) в который будут импортироваться оценки.
4. Используя <input type="file"> загружет xlsx файл с оценками.
5. Интерфейс системы позволяет определить какие столбцы в xlsx файле соответсвуют полям в коллекции `assigments`.
   Например:
     * столбец `GitHub Студента` в xlsx файле соответсвует полю `studentId
     * столбец `Результат интервью` полю `score`
     * столбец `Знание this/apply/call/bind` полю `mentorComment`
     * столбец `Знание DOM/DOM Events` полю `mentorComment`
     * столбец `Знание наследования и классов` полю `mentorComment`
     * столбец `Другие замечания` полю `mentorComment`
6. Пользователь может указать какие столбцы импортировать не нужно, выбрав для них значение "no import".
7. Данные в столбцах, для которых было выбранно поле `mentorComment` должны быть смерженны в один markdown и сохранены в поле `mentorComment`.

### Пример результата импорта в поле `mentorComment`  
```
### Знание this/apply/call/bind
Знает про call/apply/bind/this. Знает про особенности поведения arrow_functions. Умеет пользоваться.

### Знание DOM/DOM Events
Знает о onClick/addEventListener. Знает про event bubbling. Знает про querySelector/querySelectorAll. Знает про preventDefault. Умеет пользоваться.

### Знание наследования и классов
Знает наследование на синтаксисе ES2015. Немного запутался при написании наследования на синтаксисе ES5.

### Другие замечания
n/a
```
Значение 'n/a' проставляется в случает отсутствия данных в данном столбце для данного студента.

### Примеры xlsx (реальные github аккаунты студентов и менторов были удалены )
https://drive.google.com/open?id=1klJ6KqmWlslRa557Kc9P8X4SQgyVH3nj

### Обработка ошибок
Импорт данных не происходит и показывается ошибка если:
1. xlsx файл содержит повторяющиеся строки для одно и тогоже студента. Ошибка - `"student duplicate - ${student GitHub}"`
2. Если студент или ментор не найден. Ошибки - `"student ${student GitHub} not found"` или `"mentor ${mentor GitHub} not found"`
3. Если столбец score содержит не целочисленное число. Ошибка - `"student ${student GitHub}" score is not a whole number`

### Схема данных

![data scheme](http://varabei.com/public/RSSchoolApp-task.png)


