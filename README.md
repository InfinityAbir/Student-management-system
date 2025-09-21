# Student Management System

A simple CRUD (Create, Read, Update, Delete) web application built with PHP, MySQL, HTML, and CSS.  
This project allows you to manage student records: add new students, view all students, edit their details, and delete entries.

---

## Features

- Add new student (name, email, phone, course)  
- View a list of all students  
- Edit details of existing student  
- Delete student records  

---

## Tech Stack

- Backend: **PHP**  
- Database: **MySQL**  
- Frontend: **HTML** & **CSS**  

---

## Prerequisites

Make sure you have:

- A web server with PHP support (e.g. Apache via XAMPP/WAMP/MAMP)  
- MySQL server  
- A modern web browser  

---

## Setup & Installation

1. Clone the repository  
   ```bash
   git clone https://github.com/InfinityAbir/Student-management-system.git
2. Copy project to your web server folder:
    - For XAMPP → htdocs
    - For WAMP → www
    - Or wherever your local server serves files from
3. Start your web and database server (Apache, MySQL).
---
## Database Setup
1. Open phpMyAdmin or MySQL shell.
2. Create a new database. For example:
   ```bash
   CREATE DATABASE student_db;
3. Select/use the database:
   ```bash
   USE student_db;
4. Create the students table:
   ```bash
   CREATE TABLE students (
      id INT(6) AUTO_INCREMENT PRIMARY KEY,
      name VARCHAR(191) NOT NULL,
      email VARCHAR(191) NOT NULL,
      phone VARCHAR(191) NOT NULL,
      course VARCHAR(191) NOT NULL
    );
5. In your PHP config file (maybe config.php or similar), update the DB credentials:
   ```bash
   $conn = mysqli_connect("localhost", "root", "", "student_db");
---
## How to Run
1. Make sure your Apache and MySQL servers are running.
2. Open your browser and go to:
    ```bash
    http://localhost/Student-management-system/
(Adjust “Student-management-system” if you named or moved the folder differently.)
3. You should see a page listing all students (if any).
Use the interface to add new students, edit existing records, or delete.
---
## 💡 Future Improvements
Some ideas to make this stronger:
- Input validation & sanitization (e.g. check email format, non-empty fields)
- Use PDO instead of mysqli for better security
- Search/filter students (by name, course, etc.)
- Pagination if there are many student records
- User authentication (login)
- Responsive frontend design
---
## 📂 Project Structure
```bash
Student-management-system/
├── index.php         # Homepage, lists students
├── add.php           # Form for adding a new student
├── edit.php          # Form for editing student details
├── delete.php        # Logic to delete a student
├── view.php          # (if separate) viewing student details
├── css/              # Stylesheets
│   └── styles.css
├── includes/         # Config or DB connection files (e.g. config.php)
└── README.md

