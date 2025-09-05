Step 1 — Create a New Table
Create a new table in lab_crud named courses.
Include fields such as: id (auto-increment primary key), code (unique course code), title, units, and created_at.
Verify the table structure in phpMyAdmin or the MySQL CLI.
Step 2 — Build a New Controller
Following the same pattern as your studentController, create a new controller file for courses. It should include all five basic operations:

Create (POST)
Read All (GET)
Read One (GET by ID)
Update (PUT)
Delete (DELETE)
Step 3 — Add Routes
Define a new route file, just like studentRoutes, but this time for courses. Mount it in your server.js under /api/courses.

Step 4 — Test in Postman
Perform a full CRUD cycle for courses:

POST a new course (e.g., code: CS101, title: Intro to CS, units: 3)
GET all courses — confirm your new record appears
GET by ID — confirm the details of a specific course
PUT to update the course (e.g., change the title or units)
DELETE the course by ID
Step 5 — Push Your Project to GitHub
Publish your work so it’s easy to share:

Initialize Git (if not already done): git init
Add a .gitignore file to exclude node_modules and .env.
Commit your changes with a clear message (e.g., “Added courses CRUD API”).
Create a repository on GitHub and push your project.
Include an .env.example file with placeholder values, but never upload your real .env.
