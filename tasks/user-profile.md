# User Profile 

### Dev Team
Lead:
Nikita Rudy @NikitaRudy Skype: rudiynikita

Devs:
### TODO ###

### Description
Необходимо реализовать возможность сохранять/изменять/удалять профайлы студентов и менторов.

## Основные данные пользователей
Все основные данные пользователей (менторов и студентов) должны хранится в коллекции `Users`.

#### Блок Personal Information 
Данные заполняют студенты и менторы.
  - firstName: string
  - lastName: string
  - firstNameNative: string
  - lastNameNative: string
  - city: string (Можно выбрать Минск, Гомель, Гродно, Могилев, Брест или должна быть возможность вписать свой город)
  - gender: male, female
  - dateOfbirth: date
  - tShirtSize: XS, S, M, L, XL, XXL, XXXL

#### Блок Education
Данные заполняют только студенты. [Данные по учебным заведениям](https://docs.google.com/spreadsheets/d/1kmho7VVh9bCQddXfkCN4CPrauAnrTpa0MH19ZvyHAoo/edit#gid=0)
  - education 
    - university: string
    - faculty: string
    - graduationYear: number
  - englishLevel: A1, A2, B1, B2, C1, C2
  
#### Блок Employment History 
Данные заполняют студенты и менторы.
  - employmentHistory: string
  - epamDetails
    - isEPAMEmployee: true/false
    - epamEmail: string
    - epamUpsaId: string
  - experience (**заполняют только менторы**)
     - yearsInFrontEnd: less then 1, 1, 2, 3, 4, 5+
     - isStudiedAtRSSchool: true/false
     - hadMentoringExperience: true/false
  - isInternshipNeeded: true/false (**заполняют только студенты**)
  - isWorkNeeded: true/false (**заполняют только студенты**)
  
#### Блок Contacts
Данные заполняют студенты и менторы.    
  - contacts
    - phone: string
    - email: string
    - skype: string
    - telegram: string
    - other: string
 
 #### Other
 Данные заполняют студенты и менторы. 
  - notes: string
  - isEmailNotificationEnabled: true/false
 
 #### Данные на основании логина в систему
  - githubId (аккаунт через который логинится пользователь)
  - firstLoginDate (дата первого логина)
  - lastLoginDate (дата последнего логина)

## Дополнительная информация в коллекции `CourseStudent`
  - status: enrolled, expelled (**может изменить только ментор или админ**)
  - statusNote: string (**может изменить только ментор или админ**)
  
## Дополнительная информация в коллекции `CourseMentor`
  - menteeCapacity: number
  - mentees: array
  - status: 
  - notesForMentees
  - assignment: 
    - stage2: true/false
    - stage3: true/false
    - mentoringTogetherWith

### Схема данных

![data scheme](http://varabei.com/public/RSSchoolApp-task.png)


