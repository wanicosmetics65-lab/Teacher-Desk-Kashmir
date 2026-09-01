<div align="center">

<img src="tdk-logo-512.png" width="120" alt="TeacherDesk Kashmir logo">

# TeacherDesk Kashmir

### A practical digital workspace for teachers.

**Plan classes. Track students. Record attendance. Manage assessments. Handle everyday school work — all in one place.**

<br>

![Status](https://img.shields.io/badge/Status-Active-5de8b0?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-Web-4f8cff?style=flat-square)
![Backend](https://img.shields.io/badge/Backend-Supabase-3ecf8e?style=flat-square)
![License](https://img.shields.io/badge/License-All%20Rights%20Reserved-f06678?style=flat-square)

</div>

---

## About

**TeacherDesk Kashmir (TDK)** is a teacher-focused web application built to make everyday classroom work simpler and more organised.

Teachers deal with attendance, student records, marks, assessments, homework, lesson planning, reports, classroom activities and school communication on a regular basis. TDK brings these workflows together into a single workspace instead of making teachers depend on multiple disconnected tools.

The project is built around a simple idea:

> **Technology should reduce a teacher's workload, not add to it.**

TDK is designed to be practical, straightforward and usable on the devices teachers already have.

---

## Why TeacherDesk Kashmir?

TDK started from real classroom problems rather than from a desire to simply build another school-management system.

Common tasks such as:

- Taking attendance
- Maintaining student records
- Recording marks
- Preparing assessments
- Tracking homework
- Planning lessons
- Managing classroom activities
- Creating reports
- Communicating school updates

can become repetitive and time-consuming when handled manually.

TDK brings these tasks into one organised platform.

### The goal

**Less paperwork. Less switching between tools. Better organisation.**

---

# Features

## 🏫 Class Management

Manage classroom information from one place.

- Create and manage classes
- Add and manage students
- Assign subjects and classroom information
- Store student roll numbers
- Switch between active classes
- Manage classroom rosters
- Compare classes
- Create seating charts
- Manage timetables

---

## 📝 Attendance

Keep attendance records digitally.

- Daily attendance marking
- Present, absent and late tracking
- Time-stamped attendance records
- Attendance statistics
- Student-level attendance history
- Yearly attendance information

---

## 📊 Assessment & Grades

Manage academic performance without maintaining separate spreadsheets.

- Grade Book
- Assessments
- Marks and percentages
- Quiz Maker
- Test Paper Generator
- Performance Analytics
- Marks → Grade conversion
- Exit Tickets
- Yearly student results

---

## 👨‍🎓 Student Management

Keep important student information organised.

- Student Profiles
- Student records
- Attendance history
- Academic results
- Behaviour tracking
- Homework tracking
- Yearly performance information
- Class-based student management

---

## 📅 Planning & Organisation

Tools for the work that happens outside the actual lesson.

- Lesson Plans
- Timetable
- Syllabus Tracker
- Class Calendar
- Quick Notes
- Daily Summary
- Resource Library
- Report Cards
- Certificates

---

## 🎲 Classroom Tools

Small tools that can make classroom activities easier.

- Random Picker
- Class Timer
- Seating Chart
- Class Polls
- Exit Tickets
- Quick classroom utilities

---

# 📢 Announcements

TDK includes a dedicated **Announcements** section for school-wide communication.

The system is intentionally simple:

**Head of Institute → Announcement → Teachers**

When the Head of Institute publishes an announcement, teachers belonging to that institute can see it from their Announcements section.

Leave-related updates can also appear there, keeping important school communication in the same place rather than creating a separate messaging system.

---

# 🏫 Head of Institute

TDK supports two account roles:

- **Teacher**
- **Head of Institute**

The Head of Institute has additional school-level management capabilities.

Depending on the configured permissions, the HOI can:

- View teachers in the institute
- Inspect teacher information
- View teacher classes
- Review student rosters
- Review attendance statistics
- Review academic results
- Manage classroom information
- Reassign classroom information
- Remove teachers
- Export teacher reports
- Send school-wide announcements
- Communicate leave-related updates

This provides a school-level view while keeping teacher workflows separate.

---

# 🔐 Data & Security

TDK uses **Supabase** with PostgreSQL and authentication.

The application uses database-level security through **Row Level Security (RLS)** to control access to institute and teacher data.

The general relationship looks like this:

```text
                    Institute
                       │
          ┌────────────┴────────────┐
          │                         │
       Teachers                 Announcements
          │
     ┌────┴────┐
     │         │
  Classes   Teacher Data
     │
  Students
     │
  Attendance
     │
 Assessments
     │
   Results
```

Teacher accounts are associated with an institute, allowing the application to distinguish between individual teacher data and institute-level information.

---

# 🏫 UDISE School Lookup

TDK supports school lookup using **UDISE codes** during registration.

Instead of requiring school information to be entered manually, the application can use the school's UDISE code to retrieve available school details.

This makes registration faster and helps teachers associate their accounts with the correct institute.

---

# 💻 Technology

TDK intentionally uses a lightweight frontend architecture.

### Frontend

- HTML5
- CSS3
- Vanilla JavaScript
- Responsive interface
- Single-file application architecture

### Backend

- Supabase
- PostgreSQL
- Supabase Authentication
- Row Level Security
- Relational database tables
- JSON-based application data where appropriate

### No complicated build system

The main application can run as a standalone HTML file without requiring a large frontend build pipeline.

This keeps the project:

- Easy to understand
- Easy to deploy
- Easy to modify
- Lightweight
- Practical for a student-built application

---

# 📱 Designed for Everyday Use

TeacherDesk Kashmir is designed to work across common devices.

**Phone · Laptop · Desktop · Classroom PC**

The interface is designed around quick access to frequently used tools, rather than forcing teachers through complicated multi-step workflows.

---

# 🧑‍🏫 Built for Teachers

TDK isn't designed around the idea of having the most features possible.

It's designed around having **useful features in the right place**.

The project focuses on everyday teacher workflows and aims to turn repetitive manual tasks into simple digital actions.

> **The teacher remains at the centre. The software simply handles the repetitive parts.**

---

# 🔬 RSBVP

TeacherDesk Kashmir is being presented through the **Rajya Stariya Bal Vaigyanik Pradarshani (RSBVP)**.

RSBVP provides a platform for presenting the project, but the project itself was built with a different purpose:

**to create a practical tool for teachers and real classrooms.**

---

# 👨‍💻 Creator

TeacherDesk Kashmir is independently developed by:

### Mohd Izhan Wani

**GMHSS Nanil**

TDK was developed as an independent project based on real classroom needs and the idea that software can make routine teaching work more manageable.

---

# 📁 Project Structure

The main application is intentionally kept simple.

```text
TeacherDesk Kashmir
│
├── TDK10.html
├── tdk-logo-512.png
└── README.md
```

The application is primarily contained within the HTML file, including its interface, styling and JavaScript functionality.

---

# 🔒 License

Copyright © 2026 **Mohd Izhan Wani**. All rights reserved.

TeacherDesk Kashmir, including its original source code, interface design, layout, branding, application logic and implementation, is the original work of Mohd Izhan Wani.

Permission is not granted to copy, redistribute, modify, rebrand, sell or publish substantial portions of the project without explicit permission from the author.

Data entered by users belongs to those users and is handled through the application's configured database infrastructure.

---

<div align="center">

## TeacherDesk Kashmir

**Built for teachers. Built from real classroom problems.**

Made with ❤️ by **Mohd Izhan Wani · GMHSS Nanil**

</div>
