Building a Student Database with PostgreSQL

Introduction
Welcome to the Building a Student Database with PostgreSQL repository! This project is part of the freeCodeCamp curriculum and demonstrates how to create and manage a student database using PostgreSQL. The repository includes SQL scripts for setting up the database, performing various operations, and sample data for testing.

Table of Contents
Introduction
Features
Technologies Used
Setup Instructions
Database Schema
Usage
Contributing
License
Acknowledgements
Features
Comprehensive SQL script to create the student database
Examples of basic CRUD (Create, Read, Update, Delete) operations
Sample data for testing and demonstration purposes
Clear instructions for setting up and connecting to the database
Technologies Used
PostgreSQL
SQL
Setup Instructions
Clone the repository:

bash
Copy code
git clone https://github.com/Hajimet3/fcc-Building-a-Student-Database-PostgreSQL.git
cd fcc-Building-a-Student-Database-PostgreSQL
Install PostgreSQL:

Follow the instructions on the official PostgreSQL website to install PostgreSQL on your system.

Create the Database:

Open your terminal and log into PostgreSQL:

bash
Copy code
psql -U postgres
Then, create the database using the SQL script:

sql
Copy code
\i students.sql
Verify the Database:

Ensure that the database has been created successfully and the tables are in place:

sql
Copy code
\c student_database
\dt
Database Schema
The database schema is defined in the students.sql script, which includes the following tables:

students
courses
enrollments
Refer to the students.sql file for detailed table structures and relationships.

Usage
Once the database is set up, you can perform various operations such as inserting, updating, deleting, and querying data. Below are some examples:

Insert a new student:

sql
Copy code
INSERT INTO students (name, age, major) VALUES ('John Doe', 20, 'Computer Science');
Update a student's information:

sql
Copy code
UPDATE students SET age = 21 WHERE name = 'John Doe';
Delete a student:

sql
Copy code
DELETE FROM students WHERE name = 'John Doe';
Query all students:

sql
Copy code
SELECT * FROM students;
Contributing
Contributions are welcome! Please fork this repository and submit a pull request with your changes. For major changes, please open an issue first to discuss what you would like to change.
