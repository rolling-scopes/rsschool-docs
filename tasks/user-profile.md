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
  - englishLevel: A1, A2, B1, B2, C1, C2
  - employmentHistory
  - isEmailNotificationEnabled
  - epamDetails
    - isEPAMEmployee
    - epamEmail
    - epamUpsaId
  - contacts
    - phone
    - email
    - skype
    - telegram
    - other
  - notes
  - registrationDate

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
  - experience
     - yearsInFrontEnd: less then 1, 1, 2, 3, 4, 5+
     - isStudiedAtRSSchool
     - hadMentoringExperience
     - notesForMentees
  - assignment: 
    - stage2: true/false
    - stage3: true/false
    - mentoringTogetherWith

### Схема данных

![data scheme](http://varabei.com/public/RSSchoolApp-task.png)


