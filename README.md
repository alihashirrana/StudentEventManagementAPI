# Student Event Management API by ALI HASHIR RANA as my CCP (Complex Computing Problem Project)

This is a complete backend RESTful API for managing student events, registrations, and feedback, built with ASP.NET Core 9.0 and Entity Framework Core. This project was created as part of the Web Engineering course built by ALI HASHIR RANA

## Features
- Full CRUD operations for Events (Create, Read, Update, Delete).
- Participant registration for events.
- Feedback submission (rating + comment) for completed events.
- Searching and sorting capabilities for events.
- Follows Clean Architecture principles.

## Technologies Used
- **Framework:** ASP.NET Core 9.0
- **ORM:** Entity Framework Core
- **Database:** SQL Server
- **API Documentation:** Swagger (OpenAPI)
- **Architecture:** Clean Architecture (API, Application, Domain, Infrastructure layers)

## Setup and Installation

### Prerequisites
- [.NET 9.0 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/9.0)
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/)
- [SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) (or another SQL Server instance)

### Step-by-Step Setup
1.  **Clone the repository:**
    ```sh
    git clone https://github.com/YourUsername/StudentEventManagementAPI.git
    ```
    (Replace with your repo URL)

2.  **Configure the database connection:**
    - Open the solution in Visual Studio 2022.
    - Navigate to the `StudentEventManagement.API` project.
    - Open the `appsettings.Development.json` file.
    - Modify the `DefaultConnection` string to point to your local SQL Server instance. The default is `Server=localhost\\SQLEXPRESS;...`.

3.  **Create the database:**
    - In Visual Studio, go to **Tools -> NuGet Package Manager -> Package Manager Console**.
    - In the console, ensure the "Default project" is set to `StudentEventManagement.Infrastructure`.
    - Run the following command to apply the migrations and create the database:
      ```powershell
      Update-Database
      ```

4.  **Run the application:**
    - Set `StudentEventManagement.API` as the startup project (it should be by default).
    - Press the green "Play" button (or F5) to launch the API.
    - A browser window should open with the Swagger UI, where you can test all the endpoints.
