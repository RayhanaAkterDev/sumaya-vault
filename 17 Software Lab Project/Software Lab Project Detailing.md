---
class: cse
title: 
course: 
chapter: 
semester: 6th
date: 
status: todo 🔖
tags:
---
# 🏥 Software Project: Hospital Management System

## 📌 Requirements

- Patients request appointments with doctors.
- Existing patient details retrieved by the system.
- New patients update their details (with assistant’s help) before requesting appointments.
- Assistant confirms/cancels appointments based on doctor’s available slots.
- Patients are informed of appointment status.

---

## ⚙️ Tools & Languages

- **Frontend**: React + Tailwind CSS
- **Backend**: Laravel (PHP) → APIs & role-based access
- **Database**: MySQL → Tables & relationships

---

## 🌍 Public Website (Static Pages)

1. **Home** – welcome, hospital intro, services overview
2. **About Us** – hospital details, mission/vision
3. **Doctors/Departments** – list of doctors with specialization
4. **Contact** – address, phone, email, emergency info
5. **Login** – entry point for all roles
6. **Register (Patient only)** – signup for new patients

---

## 🔐 Private HMS (After Login)

### 👩 Patient

7. **Patient Dashboard** – overview (profile + recent appointments)  
8. **Patient Profile** – view/update personal details & medical history  
9. **Request Appointment** – select doctor → date → slot → submit  
10. **My Appointments** – list of all appointments with status (pending/confirmed/cancelled)  

### 🧑 Assistant

11. **Assistant Dashboard** – overview (pending appointments count, recent activity)  
12. **Manage Appointments** – list of pending → confirm/cancel with actions  
13. **Patient Registration** – assist new patients to fill/update profile  

### 👨 Doctor

14. **Doctor Dashboard** – overview of today’s appointments  
15. **My Appointments** – list of confirmed appointments (by date)  

### 👨‍💻 Admin (optional but good for marks ✨)

16. **Admin Dashboard** – overview (total patients, doctors, appointments)  
17. **Manage Doctors** – add/update/remove doctors  
18. **Reports** – appointments summary, patient list, doctor workload  

---

## ✅ Page Count

- **Public Website** → 6 pages  
- **Patient** → 4 pages  
- **Assistant** → 3 pages  
- **Doctor** → 2 pages  
- **Admin** → 3 pages (optional)  

👉 Core HMS (without admin): **15 pages**  
👉 With Admin: **18 pages total**

---

