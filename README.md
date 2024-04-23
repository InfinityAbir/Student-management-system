# CRUD Application using PHP, MySQL, HTML, and CSS

This project demonstrates a simple CRUD application built with PHP, MySQL, HTML, and CSS. CRUD operations refer to Create, Read, Update, and Delete actions performed on a database.

## Getting Started

### Prerequisites

Before starting, ensure you have the following:

- Apache server with PHP support installed
- MySQL server installed
- Basic understanding of PHP, MySQL, HTML, and CSS

### Setting Up the Database

1. Create a new database named `crud_db`.
2. Create a table named `students` with the following structure:

```sql
CREATE TABLE students (
    id INT(6) AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(191) NOT NULL,
    email VARCHAR(191) NOT NULL,
    phone VARCHAR(191) NOT NULL,
    course VARCHAR(191) NOT NULL
);
