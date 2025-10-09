# 🗓 Hospital Management System – 45-Day Daily Plan

| Day | Task                                  | Focus / Learning Outcome                                                                    |
| --- | ------------------------------------- | ------------------------------------------------------------------------------------------- |
| 1   | Setup local environment               | Install PHP, Composer, Laravel, MySQL, Node, React (Vite), Tailwind; create project folders |
| 2   | Initialize Laravel & MySQL            | Create DB, configure `.env`, migrate default tables                                         |
| 3   | Scaffold React project                | Setup Vite + Tailwind, run dev server, create basic folder structure                        |
| 4   | Build Home page (static)              | React components, Tailwind styling, header/footer                                           |
| 5   | Build About page                      | Static content, navigation using React Router                                               |
| 6   | Build Doctors/Departments page        | Simple list, learn mapping arrays in React                                                  |
| 7   | Build Contact page                    | Contact form UI (no backend yet)                                                            |
| 8   | Build Login page                      | Form handling, React state, basic validation                                                |
| 9   | Build Register page (Patient)         | Form, state, validation                                                                     |
| 10  | Learn React basics                    | Props, state, components, conditional rendering                                             |
| 11  | Setup Laravel Auth                    | Install Breeze or Sanctum, create login/register endpoints                                  |
| 12  | Connect React to Laravel APIs         | Use Axios, make login/register requests, test with Postman                                  |
| 13  | Create Users table & migrations       | Add `role` field (`patient`, `doctor`, `assistant`, `admin`)                                |
| 14  | Create Patients table & migration     | Link to users, fields: phone, DOB, gender, address, medical_history                         |
| 15  | Create Doctors table & migration      | Fields: specialization, working_days, daily_start/end, slot_duration                        |
| 16  | Create Appointments table & migration | Fields: patient_id, doctor_id, date, time, status, cancel_reason                            |
| 17  | Seed demo data                        | Create sample doctors, assistant, and patients                                              |
| 18  | Test API endpoints                    | CRUD operations for users, patients, doctors, appointments                                  |
| 19  | Patient Dashboard skeleton            | Layout, header, sidebar, placeholder components                                             |
| 20  | Patient Profile page                  | Fetch profile from API, display fields, allow editing                                       |
| 21  | My Appointments page                  | Fetch patient appointments, display in table with status                                    |
| 22  | Request Appointment page UI           | Doctor select dropdown, date picker, slot picker (UI only)                                  |
| 23  | Request Appointment API               | Send request to backend, learn form submission in React                                     |
| 24  | Fetch available slots from backend    | Learn dynamic data fetching based on date & doctor                                          |
| 25  | Submit appointment request            | POST to appointments API, handle success/fail messages                                      |
| 26  | Assistant Dashboard skeleton          | Layout with pending appointments table                                                      |
| 27  | Assistant manage appointments         | Fetch pending appointments, display patient/doctor info                                     |
| 28  | Confirm appointment action            | PUT API to confirm, update table dynamically                                                |
| 29  | Cancel appointment action             | PUT API to cancel, include optional cancel reason                                           |
| 30  | Assistant register new patient        | Form for assistant to create new patient, connect to API                                    |
| 31  | Doctor Dashboard skeleton             | Layout, placeholder for today’s schedule                                                    |
| 32  | Doctor My Appointments page           | Fetch confirmed appointments for logged-in doctor                                           |
| 33  | Role-based routing                    | React Router: redirect users based on role after login                                      |
| 34  | Protect routes                        | Only allow certain roles to access certain pages                                            |
| 35  | Improve UI                            | Tailwind styling, spacing, responsive design                                                |
| 36  | Add loading states                    | Spinners for API calls, show messages on fetch error                                        |
| 37  | Validation & error handling           | Frontend form validation, backend validation for security                                   |
| 38  | Testing backend                       | Postman collection for all APIs                                                             |
| 39  | Testing frontend                      | Manual testing: request appointments, confirm, cancel                                       |
| 40  | Connect everything                    | Patient → assistant → doctor flow fully functional                                          |
| 41  | Optional Admin Dashboard              | Manage doctors, view reports (only if time)                                                 |
| 42  | Final UI polish                       | Colors, fonts, responsiveness, small animations if desired                                  |
| 43  | Create documentation                  | ER diagram, sequence diagrams, screenshots                                                  |
| 44  | Prepare demo                          | Test all flows, fix bugs, finalize project                                                  |
| 45  | Submission & backup                   | Backup code, write README, final check                                                      |
