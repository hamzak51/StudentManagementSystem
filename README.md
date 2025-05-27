**Project Title**: Student Management System (Modular Web Application with Microservices & MVC UI)

**Technologies Used**:

UI: Windows Forms (MVC Pattern)

Backend: ASP.NET Core Web API (Microservices)

Database: SQL Server (via SSMS)

**API Testing**: Postman

**Project Description**:

This project is a Student Management System that allows you to manage student and course records. It is built using a modular architecture, where the UI follows the MVC pattern using Windows Forms, and the backend is split into independent microservices (StudentService and CourseService). These services communicate via HTTP APIs and are connected to separate databases.
_______________________________
**Architecture Overview**:

Frontend - Windows Forms (MVC):

Forms --> StudentForm, CourseForm

Models --> Student.cs, Course.cs

Controllers --> StudentController.cs, CourseController.cs

Uses HttpClient to call APIs

Microservices:

1. StudentService

RESTful API with CRUD operations

Connects to StudentDB in SQL Server

2. CourseService

RESTful API with CRUD operations

Connects to CourseDB in SQL Server
_______________________________
**Database Details**

Tools Used: SQL Server Management Studio (SSMS)

Each microservice connects to its own DB:

StudentDB → Table: Students

CourseDB → Table: Courses
_______________________________
**How to Run the Project**

1) Backend Microservices
Open each API project in Visual Studio

Update appsettings.json for correct connection strings

Run StudentService and CourseService (make sure ports are not conflicting)

2) Frontend (Windows Forms App)

Open StudentManagementUI in Visual Studio

Run the form and test the UI

Make sure backend APIs are running in background

