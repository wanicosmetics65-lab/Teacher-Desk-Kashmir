<div align="center">

<img src="tdk-logo-512.png" width="120" height="120" alt="TeacherDesk Kashmir logo"/>

# TeacherDesk Kashmir (TDK)

**A complete, database-backed teacher toolkit — built by a student, for real classrooms.**

[![RSBVP](https://img.shields.io/badge/RSBVP-Science%20Exhibition-f6c343?style=flat-square)](https://ncert.nic.in)
[![Supabase](https://img.shields.io/badge/Backend-Supabase-3ecf8e?style=flat-square&logo=supabase&logoColor=white)](https://supabase.com)
[![License](https://img.shields.io/badge/License-All%20Rights%20Reserved-f06678?style=flat-square)](#license)
[![Status](https://img.shields.io/badge/Status-Active-5de8b0?style=flat-square)]()

</div>

---

## 📖 About

**TeacherDesk Kashmir (TDK)** is an all-in-one teacher productivity app built to solve a problem observed directly inside a real school — teachers spending hours every week on paperwork: attendance registers, mark sheets, lesson notes, and behavior logs.

TDK digitalises all of that into a single app that works on any phone, laptop, or classroom PC, backed by a real cloud database (Supabase/Postgres), so a teacher's data is never lost and is accessible from any device.

Built as a project entry for the **Rajya Stariya Bal Vaigyanik Pradarshani (RSBVP)** — the State-Level Children's Science Exhibition organised by NCERT, Government of India — under the theme **"STEM for Viksit and Atmanirbhar Bharat."**

> Developed entirely by **Mohd Izhan Wani**, a student at **GMHSS Nanil** — no team, no budget, just classroom problems solved with code.

---

## ✨ Features

| Category | Tools |
|---|---|
| **Daily Tools** | Attendance (with time-stamped marking), Random Picker, Timetable, Seating Chart, Class Timer |
| **Assessment** | Grade Book, Quiz Maker, Test Paper Generator, Performance Analytics |
| **Students** | Yearly Result (tap a student → full-year attendance + academic report), Behavior Tracker, Homework Tracker |
| **Planning** | Lesson Plans, Report Cards, Announcements, Certificates, Quick Notes |
| **Extras** | Class Polls, Resource Library, Student Profiles, Class Comparison, Daily Summary |
| **New Tools** | Syllabus Tracker, Marks → Grade Converter, Exit Tickets, Class Calendar |
| **Admin** | **Head of Institute** role — Inspect any teacher's classes, students, attendance %, and results across the institute; export any teacher's full report as a standalone HTML file |

---

## 🏗️ Tech Stack

- **Frontend:** Single-file HTML/CSS/vanilla JavaScript — no build step, works offline-first
- **Backend:** [Supabase](https://supabase.com) (Postgres + Auth + Row Level Security)
- **Auth:** Supabase Auth with two roles — `teacher` and `head` (Head of Institute)
- **Data model:** Relational tables for classes, students, attendance, assessments & grades; a flexible `app_data` JSON store for the rest (timetable, homework, quiz bank, resources, etc.)

---

## 🚀 Setup

1. Create a free project at [supabase.com](https://supabase.com)
2. Open **SQL Editor** → paste the contents of [`supabase_schema.sql`](./supabase_schema.sql) → Run
3. Go to **Authentication → Providers → Email** and disable "Confirm email" (for quick testing)
4. Copy your **Project URL** and **anon/publishable key** from **Settings → API**
5. Open `index.html`, find the config block near the bottom `<script>` tag, and paste in your values:
   ```js
   const SUPABASE_URL = 'https://your-project.supabase.co';
   const SUPABASE_ANON_KEY = 'sb_publishable_xxxxxxxxxxxx';
   ```
6. Open the file in any browser — sign up as **Head of Institute** first (creates your institute), then have teachers sign up under the same institute name.

No build tools, no npm install — it's a single HTML file.

---

## 🔐 Roles

- **Teacher** — manages their own classes, students, attendance, grades, and every daily tool. Data is private to them.
- **Head of Institute** — signs up once per institute, lands on the **Inspect** dashboard, and can view (read-only) every teacher's classes, student roster, attendance %, and result averages — and export any teacher's full report as an HTML file.

---

## 📂 Repo Contents

```
index.html            → the full app (rename freely, e.g. RBVPfinal.html)
supabase_schema.sql    → paste into Supabase SQL Editor once, sets up all tables + security rules
tdk-logo-512.png        → app icon / logo
```

---

## 🛡️ License

Copyright © 2025 **Mohd Izhan Wani**. All rights reserved.

TeacherDesk Kashmir — including its design, source code, layout, features, logic, and overall concept — is the sole original work of Mohd Izhan Wani. All data entered into TDK belongs exclusively to the user and is stored only in their own Supabase project.

---

<div align="center">
<sub>Built with ❤️ by Mohd Izhan Wani · GMHSS Nanil · RSBVP Project</sub>
</div>
