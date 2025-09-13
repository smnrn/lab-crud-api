This project is a **CRUD API** implementation developed as part of a laboratory activity.  
It demonstrates how to create, read, update, and delete records from a MySQL database using a Node.js Express server.  

The project includes two main resources:
- **Students**
- **Courses**

Testing was done with **Postman**, covering both successful operations and error handling.

---

##  Features

- **CRUD Operations**
  - `POST` – Create a new record
  - `GET` – Fetch records or a specific record by ID
  - `PUT` – Update an existing record
  - `DELETE` – Remove a record

- **Error Handling**
  - Missing required fields (`400 Bad Request`)
  - Duplicate records
  - Record not found

- **Database**
  - Connected to a MySQL database (`lab_crud`)
  - Includes **students** and **courses** tables

- **Server**
  - Node.js with Express
  - CORS enabled
  - Environment-based configuration

---

## 🗂️ Project Structure

lab-crud-api/
│── config/ # Database configuration
│── routes/ # API routes for students and courses
│── server.js # Main server file
│── package.json # Dependencies and scripts

## ⚙️ Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/smnrn/lab-crud-api.git
   cd lab-crud-api
Install dependencies:
   npm install

   onfigure the database connection:

Create a .env file in the root directory with:

DB_HOST=localhost
DB_USER=root
DB_PASSWORD=yourpassword
DB_NAME=lab_crud
PORT=5000

npm start
npm run dev

You should see:

🚀 Server running… (MySQL Connected, no CORS errors)


📬 API Endpoints
Students

GET /students → Get all students

GET /students/:id → Get student by ID

POST /students → Add a new student

PUT /students/:id → Update a student

DELETE /students/:id → Delete a student

Courses

GET /courses → Get all courses

GET /courses/:id → Get course by ID

POST /courses → Add a new course

PUT /courses/:id → Update a course

DELETE /courses/:id → Delete a course



📚 Learnings

From this activity, I learned:

How to implement a CRUD API using Node.js and MySQL

How to structure a Node.js project

How to test APIs using Postman

How to handle common errors (validation, duplicates, not found)

How to use GitHub for version control
