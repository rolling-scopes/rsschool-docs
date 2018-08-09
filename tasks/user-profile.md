# User Profile 

### Dev Team
Lead:
Nikita Rudy @NikitaRudy Skype: rudiynikita

Devs:
1. @OlgaMardvilko
2. @SYAA666
3. @belashjack
4. @Kochankin @nv21 @MoRain666
5. @i-runets

### Description
Необходимо реализовать возможность сохранять/изменять/удалять/просматривать данные студентов и менторов.

### В рамках этого таска необходимо реализовать следующий страницы
1. [student view / profile](https://sonejka.github.io/rs-kittens/dist/student-profile.html)
2. [mentor view / profile](https://sonejka.github.io/rs-kittens/dist/mentor-profile.html)
3. [admin view / student profile](https://sonejka.github.io/rs-kittens/dist/admin-student-profile.html)
4. [admin view / mentor profile](https://sonejka.github.io/rs-kittens/dist/admin-mentor-profile.html)

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

#### Блок Contacts
Данные заполняют студенты и менторы.    
  - contacts
    - phone: string
    - email: string
    - skype: string
    - telegram: string
    - other: string

#### Блок Education
Данные заполняют только студенты. [Данные по учебным заведениям](https://docs.google.com/spreadsheets/d/1kmho7VVh9bCQddXfkCN4CPrauAnrTpa0MH19ZvyHAoo/edit#gid=0)
  - education 
    - university: string
    - faculty: string
    - graduationYear: number
  - englishLevel: A1, A2, B1, B2, C1, C2
  - isInternshipNeeded: true/false (**заполняют только студенты**)
  - isWorkNeeded: true/false (**заполняют только студенты**)
  
#### Блок Employment History 
Данные заполняют студенты и менторы.
  - employmentHistory: string
  - epamDetails
    - isEPAMEmployee: true/false
    - epamEmail: string
    - epamUpsaId: string
  - experience
     - yearsInFrontEnd: no experience, less than 1 year, less than 2 years, 2-5 years, more than 5 years
     - isStudiedAtRSSchool: true/false
     - hadMentoringExperience: true/false
 
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
  - status: needApproval, Approved, Rejected, notActive 
  - notesForMentees
  - assignment: 
    - stage2: true/false
    - stage3: true/false
    - mentoringTogetherWith


