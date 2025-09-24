A comprehensive console-based Java application for managing students, courses, enrollments, and grades in educational institutions. This project demonstrates advanced Java programming concepts including OOP principles, file handling with NIO.2, Stream API, and design patterns.

📚 Table of Contents
Features

Screenshots

Tech Stack

Installation

Usage

Project Structure

Java Evolution

Java Platforms Comparison

Java Architecture

Windows Installation Guide

Eclipse Setup

Syllabus Mapping

Enabling Assertions

🚀 Features
Student Management
✅ Add, list, update, and deactivate students

✅ Student profiles with ID, registration number, email, and status

✅ Transcript generation with GPA calculation

✅ Enrollment date tracking using Java Date/Time API

Course Management
✅ Create and manage courses with credits, instructors, and departments

✅ Search and filter courses by instructor, department, semester using Stream API

✅ Semester-based organization with Enum implementation

Enrollment & Grading
✅ Enroll/unenroll students with business rules (credit limits)

✅ Record marks and compute letter grades with Grade Enum

✅ GPA calculation and transcript generation

✅ Polymorphic transcript views with toString() overrides

File Operations (NIO.2)
✅ Import students/courses from CSV files

✅ Export current data to text files

✅ Automated backup system with timestamped folders

✅ Recursive directory utilities for backup size calculation

Advanced Java Concepts
✅ Singleton Pattern (AppConfig)

✅ Builder Pattern (Course.Builder)

✅ Custom exceptions with proper handling

✅ Lambda expressions and functional interfaces

✅ Nested classes and enums with constructors

🛠️ Tech Stack
Language: Java SE 17

Build Tool: Standard JDK

IDE: Eclipse IDE 2023-12

Version Control: Git

File Handling: Java NIO.2

Data Processing: Stream API

Date/Time: Java Time API

📦 Installation
Prerequisites
Java JDK 17 or higher

Git (for cloning repository)

Eclipse IDE (optional, for development)

Step-by-Step Installation
Clone the repository:

bash
git clone https://github.com/yourusername/CCRM.git
cd CCRM
Compile the project:

bash
javac -d bin src/edu/ccrm/**/*.java
Run the application:

bash
java -cp bin edu.ccrm.Main
🎯 Usage
Main Menu Options
text
=== Campus Course & Records Manager ===
1. Student Management
2. Course Management  
3. Enrollment Management
4. Grade Management
5. Import/Export Data
6. Backup Utilities
7. Reports & Analytics
8. Exit
Sample Workflow
Add Students: Select option 1 → Add Student → Enter details

Create Courses: Select option 2 → Add Course → Use Builder pattern

Enroll Students: Select option 3 → Enroll Student → Choose student and course

Record Grades: Select option 4 → Enter Marks → Automatic GPA calculation

Generate Transcript: View student profile with complete academic history

📁 Project Structure
text
CCRM/
├── src/
│   └── edu/
│       └── ccrm/
│           ├── cli/               # Command-line interface
│           │   ├── CLIMenu.java   # Main menu system
│           │   └── InputHandler.java
│           ├── domain/            # Entity classes
│           │   ├── Person.java    # Abstract class
│           │   ├── Student.java   # Inheritance example
│           │   ├── Course.java    # Builder pattern
│           │   ├── Enrollment.java
│           │   ├── Semester.java  # Enum
│           │   └── Grade.java     # Enum with points
│           ├── service/           # Business logic
│           │   ├── StudentService.java
│           │   ├── CourseService.java
│           │   ├── EnrollmentService.java
│           │   └── TranscriptService.java
│           ├── io/                # File operations
│           │   ├── FileService.java      # NIO.2 operations
│           │   ├── ImportExportService.java
│           │   └── BackupService.java    # Recursive utilities
│           ├── util/              # Utilities
│           │   ├── Validator.java
│           │   ├── GPACalculator.java
│           │   └── RecursiveUtil.java   # Recursion examples
│           ├── config/            # Configuration
│           │   └── AppConfig.java # Singleton pattern
│           └── Main.java          # Application entry point
├── data/                          # Data files
│   ├── students.csv
│   ├── courses.csv
│   ├── enrollments.csv
│   └── backups/
├── docs/                          # Documentation
├── screenshots/                   # Application screenshots
├── README.md
└── USAGE.md
📜 Java Evolution Timeline
Version	Year	Key Features Introduced
Java 1.0	1996	Initial public release
Java 1.1	1997	Inner classes, JDBC
Java 1.2	1998	Collections Framework, Swing
Java 1.3	2000	HotSpot JVM
Java 1.4	2002	Assertions, NIO
Java 5	2004	Generics, Enums, Autoboxing
Java 6	2006	Scripting support
Java 7	2011	Try-with-resources, NIO.2
Java 8	2014	Lambdas, Stream API, Date/Time API
Java 9	2017	Module system
Java 11	2018	LTS, HTTP Client
Java 17	2021	Current LTS, sealed classes
⚖️ Java Platforms Comparison
Aspect	Java SE (Standard Edition)	Java EE (Enterprise Edition)	Java ME (Micro Edition)
Target Platform	Desktop applications	Enterprise/server applications	Mobile/embedded devices
Primary Use	Standalone applications	Web applications, distributed systems	Resource-constrained devices
Key Technologies	Core APIs, Swing, JavaFX	Servlets, JSP, EJB, JMS	MIDP, CDC, CLDC
Deployment	JAR files	Application servers	Mobile devices, embedded systems
Memory Footprint	Moderate	Large	Small
Example Applications	Media players, IDEs	E-commerce sites, banking systems	Mobile games, IoT devices
🏗️ Java Architecture Explained
JDK (Java Development Kit)
Purpose: Complete development environment

Components: Compiler (javac), debugger, documentation tools

Contains: JRE + development tools

JRE (Java Runtime Environment)
Purpose: Runtime environment for executing Java applications

Components: JVM + core libraries + other components

Function: Provides runtime facilities

JVM (Java Virtual Machine)
Purpose: Execute Java bytecode independently of underlying hardware

Function: Just-In-Time compilation, memory management, garbage collection

Key Feature: Platform independence through "Write Once, Run Anywhere"

Interaction Flow:
text
Java Source Code (.java) 
    → JDK (compilation) 
    → Bytecode (.class) 
    → JRE (execution) 
    → JVM (runtime) 
    → Native Machine Code
🪟 Windows JDK Installation Guide
Step 1: Download JDK
Visit Oracle JDK Downloads Page

Download Windows x64 MSI Installer (JDK 17 or higher)

Accept license agreement

Step 2: Install JDK
Run the downloaded MSI installer

Follow installation wizard (keep default settings)

Note installation directory (typically C:\Program Files\Java\jdk-17\)

Step 3: Configure Environment Variables
Open System Properties → Advanced → Environment Variables

Create new system variable:

Variable name: JAVA_HOME

Variable value: C:\Program Files\Java\jdk-17

Edit Path variable:

Add new entry: %JAVA_HOME%\bin

Step 4: Verify Installation
Open Command Prompt and execute:

cmd
java -version
javac -version
echo %JAVA_HOME%
Expected Output:

text
java version "17.0.2" 2022-01-18 LTS
Java(TM) SE Runtime Environment (build 17.0.2+8-LTS-86)
Java HotSpot(TM) 64-Bit Server VM (build 17.0.2+8-LTS-86, mixed mode, sharing)
⚙️ Eclipse IDE Setup
Step 1: Download and Install
Download Eclipse IDE for Java Developers from eclipse.org/downloads

Run the installer and select "Eclipse IDE for Java Developers"

Choose installation folder and complete setup

Step 2: Create New Project
Launch Eclipse IDE

File → New → Java Project

Project name: CCRM

Use default JRE (Java SE-17)

Finish project creation

Step 3: Import Source Code
Right-click src folder in project explorer

Import → File System → Browse to project source folder

Select all Java files and finish import

Step 4: Configure Build Path
Right-click project → Build Path → Configure Build Path

Libraries tab → Ensure JRE System Library is correct

Source tab → Verify source folders are properly set

Step 5: Run Configuration
Run → Run Configurations → Java Application → New

Name: CCRM Main

Project: CCRM

Main class: edu.ccrm.Main

Apply → Run

📚 Syllabus Topic Mapping
Java Concept	Implementation Location	Specific Example
OOP Principles	domain/Person.java	Abstract class with inheritance
Encapsulation	domain/Student.java	Private fields with public getters/setters
Inheritance	domain/Student.java extends Person.java	Method overriding
Polymorphism	service/TranscriptService.java	Interface-based implementation
Abstraction	domain/Person.java	Abstract methods
Singleton Pattern	config/AppConfig.java	Private constructor, static instance
Builder Pattern	domain/Course.java	Inner Builder class
Exception Handling	service/EnrollmentService.java	Custom exceptions with try-catch
Stream API	service/CourseService.java	filter(), map(), collect() operations
Lambda Expressions	util/Comparator.java	Custom sorting with lambdas
NIO.2 File Operations	io/FileService.java	Files.copy(), Path operations
Date/Time API	domain/Student.java	LocalDate for enrollment dates
Enums	domain/Grade.java	Enum with constructors and methods
Recursion	util/RecursiveUtil.java	Directory size calculation
Generics	service/BaseService.java	Generic CRUD operations
⚠️ Enabling Assertions
Command Line Compilation and Execution:
bash
# Compile with assertions enabled
javac -source 1.8 -d bin src/edu/ccrm/**/*.java

# Run with assertions enabled
java -ea -cp bin edu.ccrm.Main
Eclipse IDE Configuration:
Run → Run Configurations → Java Application

Select your main class configuration

Arguments tab → VM arguments: -ea

Apply → Run

Sample Assertion Usage in Code:
java
public void enrollStudent(Student student, Course course) {
    // Precondition assertions
    assert student != null : "Student cannot be null";
    assert course != null : "Course cannot be null";
    assert student.getStatus().equals("ACTIVE") : "Only active students can enroll";
    
    // Business logic with invariant assertions
    int newCreditTotal = calculateTotalCredits(student) + course.getCredits();
    assert newCreditTotal <= 24 : "Credit limit exceeded";
    
    // Enrollment implementation
    // ...
}
🔧 Building from Source
Prerequisites:
JDK 17 or later

Git

Steps:
bash
# Clone repository
git clone https://github.com/yourusername/CCRM.git
cd CCRM

# Compile all source files
find src -name "*.java" > sources.txt
javac -d bin @sources.txt

# Run application
java -cp bin edu.ccrm.Main
🤝 Contributing
Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

Development Workflow:
Fork the repository

Create a feature branch (git checkout -b feature/amazing-feature)

Commit your changes (git commit -m 'Add amazing feature')

Push to the branch (git push origin feature/amazing-feature)

Open a Pull Request

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

👥 Acknowledgments
Oracle Java Documentation

Java Platform Standard Edition Technical Documentation

Eclipse Foundation for the excellent IDE

Stack Overflow community for programming insights

