# Institute_management_Software
Overview
This project is a web application for managing an institute's operations, including students, courses, and instructors. It is built using Spring Boot and Thymeleaf and follows the MVC design pattern. The system allows CRUD operations, relationships management, and provides a user-friendly dashboard.

---

 Features

 Core Features:
- Student Management: Add, edit, view, and delete students.
- Course Management: Add, edit, view, and delete courses.
- Instructor Management: Add, edit, view, and delete instructors.
- Relationships:
  - Assign students to courses.
  - Assign instructors to courses.
- Dashboard:
  - Display total counts of students, courses, and instructors.
- Search*:
  - Search students by name or course.
  - Search courses by instructor name.

 Optional Features:
- Pagination and sorting for student and course lists.
- Admin authentication using Spring Security.

---

 Technologies Used

-   Backend: Spring Boot (Spring MVC, Spring Data JPA)
- Frontend: Thymeleaf, Bootstrap
- Database: MySQL
- Tools: Maven,Eclipse

---

 Step 2: Set Up the Database
1. Create a MySQL database:
   ```sql
   CREATE DATABASE institute_management;
   ```
2. Configure the database in `src/main/resources/application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/institute_management
   spring.datasource.username=username
   spring.datasource.password=password
   ```
3. Optional: Use the provided `schema.sql` and `data.sql` files to manually set up tables and sample data:
   - Place `schema.sql` and `data.sql` in `src/main/resources/`.
   - Spring Boot will automatically execute them during startup.

 Step 3: Build and Run the Application
```bash
mvn clean install
mvn spring-boot:run
```

 Step 4: Access the Application
- Open your browser and visit: `http://localhost:8080/`.



 Project Structure

src/
  main/
    java/com/example/institute/
      controller/       # Controllers for handling HTTP requests
      entity/           # Entity classes (Student, Course, Instructor)
      repository/       # Spring Data JPA repositories
      service/          # Service classes for business logic
    resources/
      templates/        # Thymeleaf templates for UI
        students/       # Student-related HTML files
        courses/        # Course-related HTML files
        instructors/    # Instructor-related HTML files
      static/           # Static assets (CSS, JS, images)
      application.properties  # Application configuration


 Usage

 Access Dashboard
Visit `http://localhost:8080/` to see the dashboard with total counts of students, courses, and instructors.

 Manage Students
- URL: `http://localhost:8080/students`
- Add, edit, delete, and search students.

 Manage Courses
- URL: `http://localhost:8080/courses`
- Add, edit, delete, and search courses.

 Manage Instructors
- URL: `http://localhost:8080/instructors`
- Add, edit, and delete instructors.



 Future Improvements
- Add authentication for admin access.
- Implement pagination and sorting.
- Enhance UI with more dynamic features.


 Contact
For any queries or suggestions, feel free to reach out:
- Email -  siddhukhokle68506@gmail.com
- Mobile no- 7448299839


How to Use This File
1. Save the file as `README.md` in the root directory of your project.
2. Update placeholders like `<repository-url>` and `path-to-screenshot-` with actual values.
3. Optionally, include screenshots for better presentation.

