# Library Management System (Flask, MySQL)

A web-based Library Management System developed using Python, the Flask microframework, MySQL for database management, and HTML/CSS for the frontend. Features include book management (add, delete, issue, return), search functionality, and distinct interfaces for administrators (full access) and regular users (search only).

## Features

* **Admin User:** Full access to add, delete, issue, return, and search books. Also can view users with overdue books.
* **Regular User:** Ability to search for books.

## Technologies Used

* Python
* Flask
* MySQL
* HTML
* CSS

## Setup Instructions

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/AasthathecoderX/Library-Management-System
    cd Library-Management-System
    ```

2.  **Install dependencies:**
    ```bash
    pip install flask
    pip install mysql-connector-python
    ```
    *(Make sure you have Python and pip installed on your system.)*

3.  **Database Setup:**
    * Ensure you have MySQL installed and running.
    * Create a new database for the library management system (e.g., `library`).
    * Update the database connection details in your Flask application configuration file.

4.  **Run the Flask application:**
    ```bash
    python app.py
    ```
    *(Replace `app.py` with the name of your main Flask application file if it's different.)*

5.  **Access the application:**
    Open your web browser and navigate to `http://127.0.0.1:5000/` (or the address your Flask application is running on).

## Database Schema

```sql
-- Example SQL CREATE TABLE statements
CREATE TABLE book (
  `SL.NO` VARCHAR(1024),
  `A/c No` VARCHAR(1024),
  `Title` VARCHAR(1024),
  `Author` VARCHAR(1024),
  `Edition/Year` VARCHAR(1024),
  `Publication` VARCHAR(1024)
);



CREATE TABLE issue(
Student_Name varchar(100),
Reg_no varchar(100),
AC_No varchar(100),
Title varchar(100),
Author varchar(100),
Issue_Date varchar(100)
);

CREATE TABLE returnb(
Student_Name varchar(100),
Reg_no varchar(100),
AC_No varchar(100),
Title varchar(100),
Author varchar(100),
Return_Date varchar(100)
);
