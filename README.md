🚀 LabourIQ — Online Job Portal System
JavaFX Desktop Application

LabourIQ is a full-featured JavaFX-based desktop job portal application that connects Employers, Job Seekers, and Admins through role-based dashboards.
It is designed following OOP principles, MVC architecture, and DAO pattern, and fully satisfies GUVI Java Project requirements.

📌 Project Highlights

Desktop-based application using JavaFX

Role-based authentication and authorization

Clean separation of concerns (MVC + DAO)

Lightweight SQLite database with auto-initialization

Built using modern Java (17) and Maven

⭐ Key Features
👨‍💼 Employer Module

Post new job openings

Update and manage job listings

View job applications

Accept / reject candidates

Send messages to job seekers

🧑‍💻 Job Seeker Module

Search jobs with filters

Apply for jobs (resume upload supported)

Track application status

Manage profile details

Message employers

🛡️ Admin Module

Approve or reject job postings

Manage users (view, update roles, delete)

Monitor platform activity

View job and user statistics

🔧 Technology Stack
Core Technologies

Java 17

JavaFX 19

SQLite (File-based database)

JDBC

Maven

Architecture & Design

MVC Architecture

DAO Pattern

Object-Oriented Programming (OOP)

Development Tools

IntelliJ IDEA

Git & GitHub

JavaFX Maven Plugin

## 📁 Project Structure


labouriq/
├── pom.xml
├── LICENSE
├── README.md
├── .gitignore
├── FOLDER_STRUCTURE.md
│
├── database/
│   └── labouriq.db              # Auto-created by DBInit
│
└── src/
    └── main/
        ├── java/
        │   └── com/labouriq/
        │       ├── controllers/
        │       │   ├── AdminController.java
        │       │   ├── EmployerController.java
        │       │   ├── JobSeekerController.java
        │       │   ├── LoginController.java
        │       │   ├── SignupController.java
        │       │   ├── FXRouter.java
        │       │   └── ...
        │       │
        │       ├── dao/
        │       │   ├── UserDAO.java
        │       │   ├── JobDAO.java
        │       │   ├── ApplicationDAO.java
        │       │   └── MessageDAO.java
        │       │
        │       ├── db/
        │       │   ├── DBConnection.java
        │       │   └── DBInit.java
        │       │
        │       ├── model/
        │       │   ├── User.java
        │       │   ├── Job.java
        │       │   ├── Application.java
        │       │   └── Message.java
        │       │
        │       └── MainApp.java
        │
        └── resources/
            ├── database/
            │   └── database.sql
            │
            ├── fxml/
            │   ├── login.fxml
            │   ├── signup.fxml
            │   ├── admin_dashboard.fxml
            │   ├── employer_dashboard.fxml
            │   ├── jobseeker_dashboard.fxml
            │   ├── post_job.fxml
            │   └── ...
            │
            ├── css/
            │   └── styles.css
            │
            └── images/
                └── branding & screenshots



🚀 Build & Run Instructions (GUVI Reviewers)
✅ Prerequisites

Java 17 installed

Maven installed and added to PATH

IntelliJ IDEA (recommended)

▶️ Run the Application

From the project root directory:

mvn clean compile
mvn javafx:run

🔄 What Happens Automatically

SQLite database is initialized

Required tables are created

JavaFX modules are loaded

Login screen is launched

🗄️ Database Auto-Initialization

Database file is created automatically using DBInit.java

SQL schema executed from:

src/main/resources/database/database.sql

🔑 Default Demo Accounts
Role	Email	Password
Admin	admin@demo	admin123
Employer	employer@demo	emp123
Job Seeker	seeker@demo	seek123
🔮 Future Enhancements

Email notifications

Resume parsing

Advanced job recommendation system

Analytics dashboard

Deployment packaging (JAR / EXE)

👨‍💻 Author

Shivam Kumar
B.Tech – Computer Science
Java | JavaFX | JDBC | SQLite

📜 License

This project is licensed under the MIT License.
See the LICENSE file for more details.
