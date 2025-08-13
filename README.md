# 🎓 FYP1 Management System

This project is a comprehensive, role-based web application designed to streamline and manage the Final Year Project 1 (FYP1) proposal lifecycle. The system provides a centralized platform for Admins, Students, Supervisors, Evaluators, and Committee members.
<br><br>

### ✨ Features
The system provides distinct functionalities tailored to five different user roles:

-   **👤 Admin Portal**:
    -   **Dashboard**: View system-wide statistics (total programs, lecturers, committee members).
    -   **Program Management**: Full CRUD (Create, Read, Update, Delete) functionality for academic programs.
    -   **Lecturer Management**: Full CRUD functionality for lecturer accounts.
    -   **Committee Management**: Assign or revoke committee roles for lecturers.

-   **👨‍🎓 Student Portal**:
    -   **Self-Registration**: New students can create an account and enroll in an academic program.
    -   **Proposal Submission**: Submit FYP proposals, including title, project type (Research/Development), and supporting documents.
    -   **Supervisor Selection**: Select a preferred supervisor from a list of eligible lecturers.
    -   **Status Tracking**: View the real-time status of proposals (e.g., Pending, Accepted, Accepted with Conditions, Rejected).
    -   **Feedback & Resubmission**: View evaluator comments and resubmit proposals if required.

-   **👨‍🏫 Supervisor Portal**:
    -   **Dashboard**: View supervised proposals and pending student requests.
    -   **Student Management**: View a list of supervised students by semester and session.
    -   **Proposal Review**: View student proposals and provide initial comments before formal evaluation.
    -   **View Evaluations**: Access final evaluation results and comments for their students.

-   **📝 Evaluator Portal**:
    -   **Dashboard**: View a list of all proposals assigned for evaluation.
    -   **Proposal Evaluation**: Download proposal documents, evaluate the work, and submit a status (Accepted, Accepted with Conditions, Rejected) along with detailed comments.

-   **👥 Committee Portal**:
    -   **Dashboard**: A central hub for managing domains, students, proposals, and approvals.
    -   **Domain Assignment**: Assign research or development domains to lecturers.
    -   **Student Management**: View and manage student registrations.
    -   **Proposal Management**: Oversee all submitted proposals, view details, and filter by semester/session.
    -   **Evaluator Assignment**: Assign two evaluators to each proposal, ensuring supervisors do not evaluate their own students.
    -   **Supervisor Approval**: Review and approve/reject students' supervisor selections.
<br>

### 🛠️ Technical Overview
-   **Framework**: ASP.NET Core MVC (.NET 9)
-   **Language**: C#
-   **Database**: Microsoft SQL Server (localdb)
-   **ORM**: Entity Framework Core (Code-First Approach)
-   **Frontend**: Razor Pages, Bootstrap 5, HTML/CSS, JavaScript, jQuery
-   **Authentication**: ASP.NET Core Identity (Role-based)
-   **IDE**: Microsoft Visual Studio 2022
<br>

### 📁 File Structure
The project is submitted as a `.zip` archive containing:
-   **`FYP1System.sln`**: The main Visual Studio Solution file to open the project.
-   **FYP1System Folder**: Contains the complete ASP.NET Core application.
-   **`Report.pdf`**: The full academic report detailing the project's design, features, and implementation.
-   **`SDD.pdf`**: The Software Design Document with detailed system architecture, diagrams, and data dictionary.
<br>

### 🚀 Getting Started: Setting Up Locally

This application is designed to run on a local machine. Follow these steps to set up and run the project.

> **Prerequisites:**
> 1.  **.NET 9 SDK**: [Download here](https://dotnet.microsoft.com/download/dotnet/9.0)
> 2.  **Visual Studio 2022**: [Download here](https://visualstudio.microsoft.com/downloads/). Ensure the **"ASP.NET and web development"** workload is installed.
> 3.  **Microsoft SQL Server**: A `(localdb)\mssqllocaldb` instance is required, which is typically installed with Visual Studio.

**Step-by-Step Guide:**

1.  **📂 Extract Project Files**
    -   Download and unzip the project archive (`FYP1System.zip`) to a local directory.

2.  **✏️ Open the Solution**
    -   Launch Visual Studio 2022.
    -   Open the solution file **`FYP1System.sln`** from the extracted directory.
    -   Visual Studio will automatically restore all the required NuGet package dependencies.

3.  **🗃️ Create and Seed the Database**
    -   In Visual Studio, go to **Tools > NuGet Package Manager > Package Manager Console**.
    -   Once the console is ready, run the following command. This will connect to your local SQL Server instance, create the database, apply the schema, and populate it with initial data (including user roles and sample accounts).
        ```powershell
        Update-Database
        ```

4.  **▶️ Run the Project**
    -   Press **F5** or click the green run button (with "https" profile) in the main toolbar.
    -   Visual Studio will build the project, start the Kestrel web server, and automatically open the application's login page in your default browser.
<br>
