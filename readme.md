
Project Overview

- This project demonstrates the basics of CRUD operations (Create, Read, Update, Delete) using **Express.js** and **MySQL**.  
It provides two main resources the students  and courses. Each had full CRUD endpoints that can be tested with Postman.  The goal of this project is to understand how APIs work, 
how to connect Node.js to a MySQL database.

SetUo Steps
1. Install the necessary software like (Node.js, Git bash, Postman, Vs Code, Xampp)
2. Open XAMPP and start Apache and MySQL.
3.  Go to phpMyAdmin (`http://localhost/phpmyadmin`).
4.  Create a **user account** and a database called "lab_crud".
5.  Create two tables:
   
       - students** → `id, name, email, course, year_level`  
       - courses** → `id, code, title, units`
     
6. In your project folder, update `.env` file with your database credentials:
   
   DB_HOST=localhost
   DB_USER=yourUser
   DB_PASS=yourPassword
   DB_NAME=lab_crud
   PORT=3000
   
7. Run the project in terminal (git Bash):

    npm run dev

8. Test in browser: http://localhost:3000/api/health

   - If it shows "ok" or "connected", the setup is successful.
  

API Endpoints

Studetns:

 - POST {{baseUrl}}/students → Add a new student
  
 - GET {{baseUrl}}/students → Get all students

 - GET {{baseUrl}}/students/:id → Get student by ID

 - PUT {{baseUrl}}/students/:id → Update student by ID

 - DELETE {{baseUrl}}/students/:id → Delete student by ID


Courses:

  - POST {{baseUrl}}/courses → Add a new course

  - GET {{baseUrl}}/courses → Get all courses

  - GET {{baseUrl}}/courses/:id → Get course by ID

  - PUT {{baseUrl}}/courses/:id → Update course by ID

  - DELETE {{baseUrl}}/courses/:id → Delete course by ID

Conclusion write-up (3–5 sentences): your reflections on errors faced and lessons learned.
- ## 📝 Reflection, Challenges Faced, and Lessons Learned

In this Activity, I learned how to make a CRUD API using Express.js and MySQL. The biggest challenge I faced was that XAMPP would not run properly. When I changed the ports, MySQL 
worked but phpMyAdmin would not open. I kept trying until I found a way to fix it so both could run. I also had some errors in Postman when testing, like duplicate emails or 
missing fields, but I realized these were expected because of the validation in the code. From this activity, I learned how CRUD works with HTTP methods, 
how to organize code with routes and controllers, and how to test APIs in Postman. 








