Bug Tracking System

This project is a web-based Bug Tracking System built using ASP.NET Core MVC. It helps teams to manage software bugs efficiently through role-based login, issue tracking, and a clean user interface.

FEATURES:

1.Admin and Employee login

2.Add, view, edit, and delete bugs

3.Dashboard for Admin and Employee roles

4.Bug fields include Title, Description, Status, Severity, AssignedTo

5.Responsive user interface using Bootstrap

6.Local database integration with Entity Framework Core

TECHNOLOGIES USED:

1.ASP.NET Core MVC

2.Entity Framework Core

3.SQL Server (LocalDB)

4.Razor Views

5.Bootstrap 5

6.Visual Studio Code

7.Git and GitHub

Database Schema (Bug Table)

BugId (Primary Key)
Title
Description
Status (Open, In Progress, Closed)
Severity (Low, Medium, High)
AssignedTo
CreatedAt

HOW TO RUN PROJECT LOCALLY:

1.Clone the repository from GitHub

2.Open the folder in Visual Studio Code

3.Restore packages and build the solution

4.Use the following commands to set up the database:

    (i)dotnet ef migrations add InitialCreate

    (ii)dotnet ef database update

5.Run the application with:

    (iii)dotnet run

6.Open your browser and go to http://localhost:5000

Sample Login Credentials

Admin
Email: admin@example.com
Password: Admin@123

Employee
Email: user@example.com
Password: User@123

FUTURE IMPROVEMENTS:

1.Email notifications for new or updated bugs

2.Filters and search options for bug list

3.Export bug data as CSV or PDF

4.Add bug change history or activity log


Steps to Deploy the Application to Azure App Service

1.Open the project in Visual Studio or Visual Studio Code

2.Ensure the project builds and runs successfully on your local machine

3.Login to your Azure account using the Azure CLI or inside Visual Studio

4.Create a new Azure App Service (choose ASP.NET Core runtime)

Publish the project:

In Visual Studio: Right-click the project > Publish > Select Azure > Choose your App Service

In Visual Studio Code: Use Azure App Service extension to deploy

Configure the connection string for the database in Azure portal if required

After publishing, test the application using the Azure-provided URL