# Online Examination System

## 📌 Team Members
- **Aliaa Mohammed**  
- **Aliaa Mamoon**  
- **Aya Abdelmageed**  
- **Aya Muhammed**  

## 📝 Project Overview
### 📖 Introduction
The **Online Examination System** is designed to streamline the examination process by automating exam creation, student management, and result processing. The system ensures **secure data handling**, **efficient query execution**, and **comprehensive reporting** for ITI admins and instructors.
## 🎥 Demo
[Click here to watch the demo video on YouTube](https://www.youtube.com/watch?v=XXr9fmmHlLM)

### 🎯 Objectives
- ✅ Automate the examination process.
- ✅ Manage student registration, Exam attendance, and grading.
- ✅ Secure and optimize data storage and retrieval.
- ✅ Generate insightful reports for system administrators and instructors that can be export into Excel, word, or PDF files.

## 🛠 Technologies Used
- **📂 Database**: MS SQL Server
- **💻 Frontend**: Windows Forms (.NET Framework)
- **⚙️ Backend Tools**: Node.js & Python *(Used for web scraping to collect questions)*
- **📊 Diagramming Tools**:
  - 🖊️ *Draw.io*: Used for creating the **Entity-Relationship Diagram (ERD)**
  - 🎨 *Figma*: Used for mapping the **ERD**

## 🌟 Features of the System

- 👥 **User Management**: Manages students, instructors, and admins.
- 📜 **Exam Management**: Allows instructors to create and manage exams.
- 📚 **Question Bank**: Stores various types of questions for each course.
- 📊 **Student Tracking**: Monitors student enrollment in courses and exams.
- 🏆 **Grading & Results Processing**: Automatically calculates and stores results.
- 📑 **Reporting Module**: Generates reports related to student performance, exam details, and course information.

## 🖥️ **Dashboards**
The system includes specialized dashboards tailored to each user role, providing access to key information and functionalities:

### 1. **Admin Dashboard**
The **Admin Dashboard** is designed for system administrators to manage and oversee the entire examination system. It provides access to key metrics and insights:

- 📊 **Branch Management**: Admin can manage the different branches of the institution.
- 🔍 **Search Functionality**: Quickly search for students, instructors, tracks, courses, and more.
- 📚 **Course and Track Management**: Admins can add, update, or delete tracks and courses.
- 📝 **CRUD Operations**: Admins can perform CRUD operations on courses and tracks as well as branches.
- 📈 **Reports**: Generate detailed reports on student performance, exam data, and more.

### 2. **Instructor Dashboard**
The **Instructor Dashboard** is tailored for instructors to manage exams and question banks:

- 📝 **Exam Creation**: Allows instructors to create, modify, and schedule exams.
- 📚 **Question Bank Access**: Instructors can add, update, or delete questions in the bank.
- 📊 **Reports**: Generate reports on student exam results and grading.
- 🎓 **Student Enrollment**: View student enrollment for the courses they teach through reports.

### 3. **Student Dashboard**
The **Student Dashboard** is designed for students to interact with the system and track their exam activities:

- 📝 **Take Exams**: Students can view and take available exams.
- 📋 **Attended Exams**: Display a list of exams that the student has attended, along with their results and grades.
- ⏳ **Upcoming Exams**: Students can view upcoming exams of the courses which they are enrolled in, with details on dates and times, so they can plan ahead.

## 📊 Reporting Capabilities
The system can generate reports for with different types to export them:
- 📌 Students' details filtered by department.
- 📌 Students' grades for each enrolled course.
- 📌 Instructors' courses and the number of students enrolled in each.
- 📌 Course topics.
- 📌 Generated exam details, including questions and choices.
- 📌 Students' exam answers and grades.

## 🏗️ Project Architecture

The **Online Examination System** follows a layered architecture for better maintainability, scalability, and separation of concerns. The architecture is divided into **three main layers**:

### 1. **Data Access Layer**
This layer is responsible for interacting with the database. It handles **data retrieval** and **data manipulation** operations from the SQL Server database using **ADO.NET**. It abstracts the database operations and ensures that the higher layers (Business Logic and Frontend) are not directly exposed to the database complexities.

- **Responsibilities**:
  - Communicates with the database.
  - Executes SQL queries and stored procedures.
  - Handles CRUD operations on database tables.

### 2. **Business Logic Layer**
The **Business Logic Layer** contains the core functionalities of the system, such as **data processing**, **validation**, and **business rules**. It is responsible for interacting with the Data Access Layer to retrieve or manipulate data and providing the results to the Frontend Layer. 

- **Responsibilities**:
  - Contains the application’s business rules and logic.
  - Interacts with repositories to retrieve and process data.
  - Implements workflows like exam creation, student management, and result calculation.

### 3. **Frontend Layer**
The **Frontend Layer** provides the user interface, built using **Windows Forms** in the **.NET Framework**. It allows users (students, instructors, and administrators) to interact with the system through **forms**, **buttons**, and **dialogs**. It sends requests to the **Business Logic Layer** and displays the results to the users.

- **Responsibilities**:
  - Presents data to users.
  - Sends requests to the Business Logic Layer for operations like creating exams, viewing results, and generating reports.
  - Provides an interactive UI for users to navigate through the system.

## 🗃 Database Design
### 📁 Database Structure and Filegroups
To enhance **performance, scalability, and data management**, the Online Examination System database is structured with multiple **file groups** in MS SQL Server:
- 📂 **Exam**: Holds tables related to exams, including exam and question tables.
- 📂 **Student**: Stores student-related data.
- 📂 **Instructor**: Contains instructor-related tables.
- 📂 **Main**: Holds the remaining system tables.

### 🔄 Database Operations
- 🔹 Perform **CRUD (Create, Read, Update, Delete)** operations on all tables.
- 🔹 Use **stored procedures** for optimized data retrieval and encryption.
  
## :rocket: ERD
![ERD](https://github.com/aya-abdelmageed/OnlineExaminationSystem/blob/main/diagrams/OnlineExaminationSystem.drawio.png)


###  🎥 Demo
[🎥 Watch Demo Video](https://github.com/aya-abdelmageed/OnlineExaminationSystem/blob/main/Demo/ExaminationSystemDemo.mp4)


This documentation provides an overview of the **database structure** and **functionalities** of the Online Examination System. For more details, refer to the **Demo**, **code**, and additional **documentation files** in this repository.
