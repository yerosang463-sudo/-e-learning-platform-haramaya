# 🎓 E-Learning Platform - Haramaya University

## 📋 Project Overview
A complete e-learning platform with quiz system, certificate generation, and Ethiopian payment integration.

## 🚀 Features
- ✅ User authentication (Student/Admin roles)
- ✅ Course browsing with search & filters
- ✅ Complete quiz system with timer
- ✅ Automatic certificate generation
- ✅ Ethiopian payment gateways (Telebirr, CBE)
- ✅ Admin dashboard for management
- ✅ Progress tracking

## 🛠️ Technology Stack
- **Frontend:** HTML5, CSS3, JavaScript
- **Backend:** PHP 7.4+
- **Database:** MySQL
- **Security:** PDO, bcrypt hashing, sessions

## 📁 Project Structure
e-learning-platform/
├── login.php # Authentication
├── student_dashboard.php # Student home
├── admin_dashboard.php # Admin panel
├── take_quiz.php # Quiz interface
├── certificates.php # Certificate generation
├── payment.php # Payment system
├── style.css # Styling
├── db_conn.php # Database connection
└── database/ # Database schema

## 🖥️ Installation & Setup

### 1. Server Requirements
- PHP 7.4 or higher
- MySQL 5.7 or higher
- Apache/Nginx web server

### 2. Database Setup
```sql
-- 1. Create database
CREATE DATABASE e_learning;

-- 2. Import database (use e_learning_database.sql)
-- 3. Update db_conn.php with your credentials
3. Configuration
Edit db_conn.php:
$host = 'localhost';
$dbname = 'e_learning';
$username = 'root';
$password = '';  // Your password
4. Default Accounts
Admin: admin@test.com / 123456
Student: student@test.com / 123456
🎯 Usage Demo
1.Access login.php
2.Login as student → Browse courses → Take quiz → Get certificate
3.Login as admin → Manage courses → View analytics
📊 SRS Compliance
93% of requirements implemented
Ethiopian context integration
Secure payment simulation
Responsive design
👥 Team Members
[Name 1]
[Name 2]
[Name 3]
[Name 4]
[Name 5]
📚 Course Information
Course: programming 2
Instructor: Mr.Aliy
University: Haramaya University
Submission Date: December 2025

### **PART 4: CREATE DATABASE SETUP GUIDE**

Create `DATABASE_SETUP.md`:

```markdown
# 🗄️ Database Setup Guide

## File: `e_learning_database.sql`

## 📋 Steps to Import Database:

### Method 1: Using phpMyAdmin
1. Open phpMyAdmin (http://localhost/phpmyadmin)
2. Create new database: `e_learning`
3. Click "Import" tab
4. Choose `e_learning_database.sql`
5. Click "Go"

### Method 2: Using MySQL Command Line
```bash
mysql -u root -p e_learning < e_learning_database.sql


📊 Database Structure
Tables:
├── users (id, email, password, role, full_name)
├── courses (id, title, description, price, category)
├── enrollments (user_id, course_id, enrollment_date)
├── quizzes (id, course_id, title, time_limit, passing_score)
├── quiz_questions (id, quiz_id, question_text, question_type)
├── quiz_options (id, question_id, option_text, is_correct)
├── quiz_attempts (id, user_id, quiz_id, score, percentage)
├── user_quiz_progress (user_id, quiz_id, best_score, passed)
├── transactions (id, user_id, course_id, amount, payment_method)
└── categories (id, name, description)
🔐 Default Data Included
9 sample courses (mix of free/paid)
Python course with 5-question quiz
Admin & student accounts
Sample categories
⚠️ Troubleshooting
1.Connection error: Check db_conn.php credentials
2.Tables missing: Re-import SQL file
3.Login fails: Use demo accounts provided

Please upload these to GitHub for our project submission:
1.ATTACHED: e_learning_project.zip (extract to get all PHP files)
2.ATTACHED: e_learning_database.sql
STEPS TO UPLOAD:
1.Go to github.com and login
2.Create new repository: "e-learning-platform-haramaya"
3.Upload all PHP files from the zip
4.Create README.md with the provided content
5.Upload database.sql file
6.Create DATABASE_SETUP.md file
DEMO INFO:
Start file: login.php
Admin: admin@test.com / 123456
Student: student@test.com / 123456
The teacher will check from GitHub, so make sure:
✅ All files are uploaded
✅ README is complete
✅ Database setup instructions are clear
