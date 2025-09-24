# Campus Course Records Manager

## Made by  
**Name:** Vani Priya  
**Registration Number:** 24BEY10147  
**Course:** Programming in Java  
**Course Code:** CSE2006  
**Institution:** VIT Bhopal University  
**Submission Platform:** Vityarthi  

---

## About This Project  
This is my Java programming project for managing campus courses and student records. I built this application to learn object-oriented programming and file handling in Java. This project is part of my Programming in Java course this semester, submitted through the Vityarthi platform.

---

## How to Setup and Run  

### What You Need  
- Java JDK 21 or later  
- Command Prompt or Terminal  

### Steps to Run:  
1. Download my project files  
2. Open Command Prompt  
3. Navigate to the project folder:  
   `cd Desktop\CampusCourseRecordsManager\src`  
4. Compile the code:  
   `javac -d ../out edu/ccrm/cli/CCRMApplication.java`  
5. Run the program:  

---

## Features I Implemented  

### Student Management  
- Add Student  
- List All Students  
- Update Student  
- Deactivate Student  
- Display Student Profile  

### Course Management  
- Add Course  
- List All Courses  
- Update Course  
- Deactivate Course  
- Search Courses  

### Enrollment & Grading  
- Enroll Student in Course  
- Unenroll Student from Course  
- Record Grade  

### Reports  
- Top Students by GPA  
- GPA Distribution  
- Course Statistics  
- Student Statistics  

### Backup & File Operations  
- Create Backup  
- Show Backup Directory Size  
- List Backup Files  
- Export Data  

### Search Operations  
- Search Students by Status  
- Search Students by GPA Range  
- Search Courses by Credits  

---

## Evolution of Java  
| Year | Major Java Version               | Key Features                               |  
|-------|---------------------------------|--------------------------------------------|  
| 1995  | Java 1.0                        | Released by Sun Microsystems                |  
| 2004  | J2SE 5.0                       | Introduced generics, autoboxing, enums     |  
| 2014  | Java SE 8                      | Introduced Lambdas and Stream API           |  
| 2018  | Java SE 11 (LTS)               | Modularization                              |  
| 2021  | Java SE 17 (LTS)               | Sealed classes                              |  
| 2023  | Java SE 21 (LTS)               | Virtual threads                             |  

---

## Java Platforms Comparison  

| Aspect  | Java ME           | Java SE             | Java EE                |  
|---------|-------------------|---------------------|------------------------|  
| Purpose | Mobile & Embedded | Desktop & Server    | Enterprise             |  
| Scope   | Limited API       | Full Core API       | Enterprise Extensions  |  
| Target  | IoT devices       | Applications        | Web Services           |  
| This Project | ❌              | ✅                  | ❌                      |  

---

## JDK/JRE/JVM Explanation  

### JDK (Java Development Kit)  
- Complete development package for Java programmers  
- Contains compiler (javac), tools (java, jar, javadoc)  
- Contains libraries and development files  
- Used for developing Java applications  

### JRE (Java Runtime Environment)  
- Environment to run Java applications  
- Contains JVM and core libraries  
- Used to execute Java programs (end-users need this)  

### JVM (Java Virtual Machine)  
- Executes Java bytecode  
- Loads and verifies code safety  
- Executes code line by line  
- Provides memory management with garbage collection  
- Makes Java platform-independent (Write Once, Run Anywhere)  

---

## Windows Installation Steps  
1. Download JDK 21 from Oracle website  
2. Run installer and follow setup instructions  
3. Set `JAVA_HOME` environment variable to JDK installation path  
4. Add `%JAVA_HOME%\bin` to system PATH  
5. Verify installation with:  
*(See `screenshots/java-install-verification.png`)*

---

## Eclipse Setup Steps  
1. Download Eclipse IDE for Java Developers  
2. Extract and run `eclipse.exe`  
3. Configure Installed JREs to point to JDK 21  
4. Import project as Existing Projects into Workspace  
5. Set run configuration for `CCRMApplication` main class  
*(See `screenshots/eclipse-setup.png`)*

---

## Syllabus Topic Mapping  

### 1. Java Introduction & Basics  

| Topic               | File/Class            | Method/Example          |  
|---------------------|----------------------|------------------------|  
| Java Variables & Data Types  | All domain classes    | Field declarations      |  
| Java Operators       | CCRMApplication.java  | demonstrateOperators() |  
| Java Input and Output| CCRMApplication.java  | Scanner usage           |  
| Java Comments        | All files             | Code comments           |  
| Java Expressions & Blocks | All files          | Method implementations  |  

### 2. Java Flow Control  

| Topic               | File/Class            | Method/Example          |  
|---------------------|----------------------|------------------------|  
| if-else statements   | Student.java          | enrollInCourse()        |  
| switch Statement     | CCRMApplication.java  | Menu system             |  
| for Loop            | CCRMApplication.java  | displayStudentProfile() |  
| for-each Loop       | StudentService.java   | findAll() method        |  
| while Loop          | CCRMApplication.java  | Main menu loop          |  
| break Statement     | CCRMApplication.java  | Labeled break           |  
| continue Statement  | CCRMApplication.java  | displayStudentProfile() |  

### 3. Java OOP (Basics)  

| Topic               | File/Class            | Method/Example          |  
|---------------------|----------------------|------------------------|  
| Class and Objects    | All domain classes    | Class definitions       |  
| Methods             | All classes           | Method implementations  |  
| Constructor         | All domain classes    | Constructors            |  
| Strings             | All files             | String manipulations    |  
| Access Modifiers    | All classes           | private, protected, public |  
| this keyword        | All domain classes    | Constructor usage       |  
| final keyword       | Name.java             | Immutable class         |  
| Recursion           | BackupService.java    | calculateDirectorySize()|  
| instanceof Operator | CCRMApplication.java  | demonstratePolymorphism()|  

### 4. Java OOP (Inheritance & Polymorphism)  

| Topic               | File/Class            | Method/Example          |  
|---------------------|----------------------|------------------------|  
| Inheritance          | Person.java → Student.java | extends keyword       |  
| Method Overriding    | Student.java          | displayProfile() override |  
| super Keyword       | Student.java          | Constructor super()     |  
| Abstract Class & Method | Person.java        | abstract class/methods  |  
| Interfaces          | Persistable.java      | Interface implementation|  
| Polymorphism        | CCRMApplication.java  | displayProfile() calls  |  
| Encapsulation       | All domain classes    | Getters/setters         |  

### 5. Java OOP (Other types of classes)  

| Topic               | File/Class            | Method/Example          |  
|---------------------|----------------------|------------------------|  
| Nested & Inner Class | Student.Statistics    | Static nested class     |  
| Static Class        | Comparators.java      | Static utility class    |  
| Anonymous Class     | Comparators.java      | BY_REGISTRATION_DATE    |  
| Singleton Pattern   | AppConfig.java        | getInstance() method    |  
| enum Class          | Grade.java, Semester.java | Enums with fields   |  
| enum Constructor    | Grade.java            | Enum constructors       |  
| enum String         | All enums             | toString() overrides    |  

### 6. Java Exception Handling  

| Topic               | File/Class            | Method/Example           |  
|---------------------|----------------------|-------------------------|  
| Exceptions          | Custom exception classes | Exception hierarchy     |  
| Exception Handling  | CCRMApplication.java  | try-catch blocks        |  
| try-catch           | CCRMApplication.java  | manageBackup() method   |  
| throw and throws    | Student.java          | enrollInCourse()        |  
| Custom Exceptions   | DuplicateEnrollmentException.java | Custom exception classes |  

### 7. Java Collections & I/O Streams  

| Topic               | File/Class            | Method/Example           |  
|---------------------|----------------------|-------------------------|  
| Collections Framework| All services         | ArrayList, HashMap       |  
| List Interface      | All services         | List usage               |  
| ArrayList           | StudentService.java  | students collection      |  
| I/O Streams         | BackupService.java   | Files operations         |  
| Byte-oriented streams| BackupService.java   | Files.write()            |  
| String operations   | All files            | String manipulations     |  
| Arrays              | All services         | Array operations         |  

---

## Enabling Assertions  
To enable assertions (for credit limit validation), run with the `-ea` flag:  
undefined
