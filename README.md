# Student Records Management System

A school-style **Python Flask + HTML/CSS** project.

## Storage Requirement

This project uses **Python Lists only** (no database). All lists are now
**saved to a `data.json` file** after every change and reloaded when the
server starts, so accounts, grades, schedules, subject assignments,
courses, announcements, and reports are **kept even after logging out or
restarting the server**.

## Default administrative account

Username: `admin`
Password: `admin123`

## How to run

```bash
python -m venv venv
venv\Scripts\activate        (Windows)
source venv/bin/activate       (Mac/Linux)
pip install -r requirements.txt
python app.py
```

Open: `http://127.0.0.1:5000`

## What each role can do

### Admin
- View registered users (Students table + Teachers table)
- **Add Student / Teacher accounts** directly (no signup needed)
- **Manage Courses**: add new courses (code + full program name); they
  instantly appear in signup, registration, and grade entry
- **Subjects & Teachers**: finalize which teacher handles each subject
  for each student — edit the teacher, edit the subject, or remove it
- **All Schedules**: view, add, edit, or remove any student's schedule
  entries (day, time, subject, room)
- Reset passwords, change Student IDs, change roles, delete accounts
- Post announcements and review problem reports

### Teacher
- Select students (any course) and manage them
- Add / update / delete grades (with academic period, year level, program)
- **Assign subjects** to a student under themselves — the assignment is
  saved once (finalized) and shown to the student; no repeated entry
- Post and delete class schedules for selected students
- Profile, change password, settings, report problems

### Student
- View personal academic records (grades)
- View classmates (same course + year level)
- **My Teachers & Subjects**: see every finalized subject with the teacher
  handling it, plus a list of their teachers
- View personal schedule
- Profile, change password, settings, report problems

## OOP requirements demonstrated

- Functions, Lists, Encapsulation through classes, Inheritance,
  Polymorphism, Exception Handling, Flask, HTML/CSS,
  Role-based access control
