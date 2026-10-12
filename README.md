# 🎓 Student Management System

A beginner-friendly, full-stack web application designed to manage student details efficiently. This project demonstrates full CRUD operations, database connectivity, real-time search filtering, and centralized error handling using modern Java standards.

---

## 📌 Project Overview (What I Built)

1. **Backend Layer (Spring Boot 3 & JPA):**
   - Built a RESTful architecture following the standard `Controller -> Service -> Repository -> Entity` pattern.
   - Connected to **MySQL Database** with automatic table synchronization via Hibernate.
   - Implemented server-side validation (`@NotBlank`, `@Email`, `@NotNull`) and handled errors cleanly using `@RestControllerAdvice`.

2. **Frontend Layer (HTML, CSS & JavaScript):**
   - Designed a responsive UI using external styling (`style.css`).
   - Integrated dynamic CRUD actions (Create, Read, Update, Delete) via native JavaScript Fetch API without page reload.
   - Built an instant client-side search bar to filter records in real-time.

---

## 📸 Screenshots & Demo

### 1. Main Dashboard & Student Management
> Displays student records with Register Number, Name, Email, Department, and Year alongside Add, Edit, and Delete controls.

<img width="1155" height="608" alt="Screenshot 2026-10-12 163920" src="https://github.com/user-attachments/assets/cf500de0-ccad-4f18-b307-47210b5d76f3" />


### 2. Search & Filter in Action (Filtering by CSE)
> Instantly filters matching students as the user types department or student details.
<img width="1142" height="489" alt="Screenshot 2026-10-12 163937" src="https://github.com/user-attachments/assets/4cb0c542-a5a6-499c-b5f3-ad8d3e151ea8" />


---

## 🚀 Features

- **Full CRUD Support:** Add, View, Edit/Update, and Delete students.
- **Dynamic Search:** Real-time table filtering by Reg No, Name, Email, Department, or Year.
- **Input Validation:** Prevents blank submissions and validates proper email formats.
- **Clean Structure:** Fully decoupled CSS, clean JavaScript functions, and standard Spring Boot directory setup.

---

## 🛠️ Tech Stack

- **Backend:** Java 17+, Spring Boot 3, Spring Data JPA, Hibernate
- **Database:** MySQL
- **Frontend:** HTML5, CSS3, Modern JavaScript (Fetch API)
- **Build Tool:** Maven

---

## 📋 Database Schema

**Table: `students`**

| Column | Type | Description |
|---|---|---|
| `id` | BIGINT | Primary Key (Auto-Increment) |
| `reg_no` | VARCHAR(255) | Student Register Number |
| `name` | VARCHAR(255) | Student Full Name |
| `email` | VARCHAR(255) | Unique Student Email |
| `department` | VARCHAR(255) | Department / Branch |
| `year` | INT | Academic Year (1 to 4) |

---

## 🔌 REST API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/api/students` | Fetch all students |
| `GET` | `/api/students/{id}` | Fetch a single student by ID |
| `POST` | `/api/students` | Add a new student |
| `PUT` | `/api/students/{id}` | Update an existing student |
| `DELETE` | `/api/students/{id}` | Delete a student |

---

---

## 💡 Key Architectural Highlights

* **Decoupled Architecture:** Clean separation between the client presentation layer and REST controller endpoints.
* **Database Integrity:** Automatic relational table mapping with unique constraint enforcement on student identifiers and emails.
* **Graceful Exception Handling:** Catches validation failures and constraint violations centrally, returning structured feedback instead of stack traces.
* **Responsive UI:** Clean CSS layout with intuitive action triggers (inline editing, real-time filtering, delete confirmation prompts).

---

## 🎯 What I Learned & Practiced

* Building and structuring full-stack web applications using **Spring Boot 3** and **MySQL**.
* Implementing robust backend business logic across Entity, Repository, Service, and Controller layers.
* Utilizing **Jakarta Bean Validation** alongside `@RestControllerAdvice` for centralized error responses.
* Connecting a vanilla JavaScript frontend to REST APIs using modern asynchronous `fetch` calls.

---

## 👩‍💻 Author - Bahmitha Begam

Developed as a full-stack Java learning project showcasing RESTful API design and responsive web interfaces.
