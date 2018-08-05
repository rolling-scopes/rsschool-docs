# User Profile 

### Dev Team
Lead:
Nikita Rudy @NikitaRudy Skype: rudiynikita

Devs:
### TODO ###

### Description
Необходимо реализовать возможность сохранять/изменять/удалять профайлы студентов и менторов.

### Хранимые данные
Вся базовая информация должна хранится в коллекции `Users`:
  - githubId
  - firstName
  - lastName
  - firstNameNative
  - lastNameNative
  - city
  - education
    - university
    - faculty
    - graduationYear
  - englishLevel: A0, A1, A1-A2, A2, B1, B2, C1, C2
  - phone
  - email
  - registrationDate
  - employmentHistory
  - isEPAMEmployee
  - isEmailNotificationEnabled
  - notes

Дополнительная информация в коллекции `CourseStudent`
  - isInternshipNeeded
  - isWorkNeeded
  - status
  - 
  
Дополнительная информация в коллекции `CourseMentor`
  - menteeCapacity
  - mentees
  - status
  - tshirt:
     - size: XS, S, M, L, XL, XXL, XXXL
     - fashion: male, female

### Схема данных

![data scheme](http://varabei.com/public/RSSchoolApp-task.png)


