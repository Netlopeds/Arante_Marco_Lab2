**3ISA – Laboratory Activity #2: CRUD API with Express.js and MySQL**

In this lab, I developed a basic RESTful API using Express.js as the backend framework and MySQL for data persistence. The API will manage student and course information, showcasing the four main CRUD operations: Create, Read, Update, and Delete. The activity will guide you in applying clean project organization, database connectivity, and API testing with Postman.

**Step 1: Database Setup**

Open MySQL and create a database named lab_crud.
Inside it, define two tables:
students → (id, name, age, course, created_at)
courses → (id, code, title, units, created_at)
Confirm your schema using either phpMyAdmin or the MySQL CLI.

**Step 2: Express Server Initialization**

Install and configure an Express.js project.
Use a .env file to safely store MySQL connection credentials.
When configured correctly, starting the server should display:
🚀 Server running…
✅ MySQL connected

**Step 3: Controllers**

Following the MVC(Model View Controller) -style structure, create two controllers that handle database logic:
studentController.js → For all student-related CRUD functions
courseController.js → For all course-related CRUD functions

Each controller must implement:
POST → Create a record
GET (all) → Retrieve all records
GET (by ID) → Retrieve one record
PUT → Update an existing record
DELETE → Remove a record

**Step 4: Routes**

Define separate route files:
studentRoutes.js → mounted at /api/students
courseRoutes.js → mounted at /api/courses
Register these routes in your server.js so the API can serve both endpoints.

**Step 5: Postman Testing**

Using Postman, perform a complete CRUD cycle for both entities:
Students
POST /api/students → Add new student
GET /api/students → View all students
GET /api/students/:id → Fetch a single student
PUT /api/students/:id → Edit student details
DELETE /api/students/:id → Remove a student

Courses
POST /api/courses → Add new course
GET /api/courses → View all courses
GET /api/courses/:id → Fetch a single course
PUT /api/courses/:id → Edit course details
DELETE /api/courses/:id → Remove a course

For Postman environment configure with {{baseUrl}} to simplify requests.

**Step 6: GitHub Submission**

Initialize a Git repository if not already done (git init).
Add a .gitignore file to exclude node_modules/ and .env.
Commit with a descriptive message (e.g., "Implemented CRUD API for students and courses").
Provide an .env.example with placeholder credentials (never push your actual .env).
