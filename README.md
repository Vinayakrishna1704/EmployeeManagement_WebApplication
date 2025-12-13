# EmployeeManagement_WebApplication
This is a Web Application built using ASP.NET Core (.NET 8), Entity Framework Core, and the N-Tier Architecture pattern. It demonstrates a clean and scalable structure for performing basic CRUD operations (Create, Read, Update, Delete) for Employee Management.

## 🚀 Features

Add, update, delete, and view employees

Structured using N-Tier Architecture (Business Logic , Data Access , Model)

Uses Entity Framework Core for database operations

Built with ASP.NET Core MVC

SQL Server as the database provider

Strong separation of concerns for easier maintainability and scalability

## 🛠️ Tech Stack

.NET 8 (ASP.NET Core MVC)

Entity Framework Core

SQL Server

N-Tier Architecture

Bootstrap for UI styling

##  📂 Explanation and Project Architecture

This solution follows the N-Tier Architecture pattern and is structured into two Class Library projects and one ASP.NET Core Web Application, ensuring clear separation of concerns and maintainability.

### WebApp.DataAccess
<img width="854" height="635" alt="image" src="https://github.com/user-attachments/assets/e4f7394b-8c29-4f13-94de-d67313ef47e1" />

<img width="940" height="398" alt="image" src="https://github.com/user-attachments/assets/3ddf3836-c7ef-4794-b489-710fc906f053" />


This layer is responsible for data access and database management.
It includes:

* ApplicationDbContext for database interactions

* Entity Framework Core migrations

* Code-First approach, where the database is generated based on C# models and configuration

All database-related operations are handled exclusively in this layer.

### WebApp.Model 

<img width="610" height="188" alt="image" src="https://github.com/user-attachments/assets/c9df1894-cd48-442b-9448-4dfc8d0443a0" />

<img width="428" height="289" alt="image" src="https://github.com/user-attachments/assets/d905c0ed-8d99-478d-b741-e30a7e96f324" />

<img width="940" height="427" alt="image" src="https://github.com/user-attachments/assets/309098eb-753b-4e15-aa52-fb37156a8087" />

<img width="740" height="734" alt="image" src="https://github.com/user-attachments/assets/8394143e-25a9-447d-bed8-890b0914c477" />

This layer contains the domain models used across the application.

* Defines entity classes such as Employee

* Represents table structures and relationships in the SQL database

* Acts as a bridge between the database and business logic

Each model maps directly to its corresponding database table using Entity Framework Core.

### WebApplication1 (Presentation Layer)

<img width="562" height="420" alt="image" src="https://github.com/user-attachments/assets/b9f995d0-04c8-46c2-b085-4a29605105bb" />

This is the ASP.NET Core MVC Web Application.

* Contains Controllers and Views

* Uses ORM (Entity Framework Core) to perform CRUD operations

* Interacts with the DataAccess layer through models

Responsible for handling user requests and rendering UI

## ✅ Key Benefits of This Architecture

#### * Clear separation of concerns

#### * Scalable and maintainable codebase

#### * Reusable model and data access layers

#### * Clean integration with Entity Framework Core












