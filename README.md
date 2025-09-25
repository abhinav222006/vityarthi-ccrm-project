Campus Course & Records Manager (CCRM)

## Overview

The Campus Course & Records Manager (CCRM) is a console-based Java application built to manage student records, courses, enrollments, and grades for educational institutions.
It’s designed as an end-to-end academic management system while demonstrating advanced Java SE concepts and modern software engineering practices.


---

## Features

Student Management → Add, update, search, and manage student profiles

Course Management → Build and maintain course catalogs with instructor mapping

Enrollment System → Enroll students with rules like credit limits & duplicates

Grade Management → Record marks, calculate GPAs, and generate transcripts

File Operations → Import/export data in CSV using NIO.2 APIs

Backup System → Automated backups with recursive directory traversal

Reports & Analytics → Stream API-based insights (e.g., GPA stats, top students)



---

## How to Run

Prerequisites

JDK 8 or higher

Any Java IDE (Eclipse, IntelliJ, VS Code) or just the command line


Command Line

# Compile all files
javac -d . edu/ccrm/**/*.java  

# Run the application
java edu.ccrm.CCRMApplication  

# Run with assertions enabled (recommended)
java -ea edu.ccrm.CCRMApplication

Eclipse Setup

1. Create a new Java Project


2. Import all source files, maintaining the package structure


3. Run CCRMApplication.java as Java Application


4. (Optional) Enable assertions via Run Configurations → VM arguments → -ea




---

## Java Concepts Demonstrated

OOP Principles → Encapsulation, Inheritance, Abstraction, Polymorphism

Design Patterns → Singleton (AppConfig), Builder (Student, Course)

Exception Handling → Custom exceptions + try-catch-finally

File I/O (NIO.2) → Path, Files, Streams, recursive operations

Streams & Lambdas → Filtering, mapping, sorting with concise code

Date/Time API → Registration timestamps, backup folders

Assertions → Input validation & state checks



---

## Project Structure

edu/ccrm/
├── domain/        # Core domain classes (Student, Course, etc.)

├── service/       # Business logic layer

├── io/            # File operations (CSV, backups)

├── util/          # Utilities (Validation, Comparators)

├── config/        # Singleton AppConfig

├── cli/           # Command Line Interface

└── CCRMApplication.java  # Main entry point


---
## Sample Data

Pre-loaded 3 students with different GPAs

Pre-loaded 3 courses from different departments

Sample enrollments & grades

Extra test data available in test-data/ directory



---
## Future Enhancements

Database integration with JDBC

Web interface (Spring Boot + REST APIs)

Advanced reporting with charts/graphs

Email notifications

Academic calendar integration



---

## Troubleshooting

ClassNotFoundException → Check compilation & package structure

File Not Found → Ensure data/backup directories exist

Assertion Errors → Run with -ea flag

Memory Issues → Use -Xmx512m for larger datasets



---

##
License

This project is built for educational purposes as part of the Java SE learning curriculum.
