# 🏫 Debbie School of Mind Database Project

Welcome to the **Debbie School of Mind Database System**!  
This project is a relational database design built to manage users, students, employees, courses, enrollment, grades, and departments. It is modeled using an **Entity-Enhanced Relationship Diagram (EERD)** and implemented with **11 tables**. 🎓📊

---

## 📊 EER Diagram
The EER Diagram shows how the 11 tables are related.  
//might come back and add final picture of the diagram

---

## 🗂 Database Tables
This project contains **11 tables** with primary key, foreign key, and check constraints:

| Table Name           | Description |
|----------------------|-------------|
| `user`              | Stores system users (students, employees, admins) |
| `student`           | Stores student-specific details linked to `user` |
| `employee`          | Stores employee details (faculty, staff) linked to `user` |
| `course_enrollment` | Links students to courses with uniqueness enforced |
| `course_faculty`    | Links faculty (employees) to course sections |
| `letter_grade`      | Stores letter grades for student enrollments |
| `course`            | Stores course information (name, description) |
| `department`        | Stores academic departments |
| `course_section`    | Represents course offerings by semester |
| `semester`          | Stores semester details (Fall, Spring, Summer + Year) |
| `course_room`       | Stores room assignments and capacities for sections |

---

## 🔑 Key Features
- ✅ **Primary and Foreign Keys** for relationships  
- ✅ **Unique constraints** (e.g., one student can’t enroll twice in the same course)  
- ✅ **Audit columns** (`audit_user_id`, `audit_timestamp`) for tracking changes  
- ✅ **Check constraints** (e.g., grade values must be `A, B, C, D, F, W `)  
- ✅ **Many-to-Many relationships** resolved with associative tables like `course_enrollment` and `course_faculty`  

---

## 🛠 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/rnegrete01/Debbie_school_of_minds_college_v1
