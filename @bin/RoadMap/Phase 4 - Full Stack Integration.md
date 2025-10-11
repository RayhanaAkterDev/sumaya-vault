# 🔄 Phase 4: Full Stack Integration (React + Laravel)

> **🎯 Goal:** Connect a **React frontend** with a **Laravel backend** using **RESTful APIs**. Handle **authentication**, manage **CORS**, perform **database operations**, and build a fully functional full-stack application.
> ⏳ **Suggested Duration:** 1 Oct 2025 → 30 Nov 2025 (2 months)

---

## ✅ Laravel API Backend (Preparation)

### 🎯 Learning Topics
- Laravel API routes & controllers    
- JSON responses with status codes    
- API Resources & API Resource Collections    
- Form validation and error handling for APIs    

### 🧩 Mini Tasks
- Create an API endpoint for blog posts    
- Add validation and return JSON error messages    
- Create resource controller and resource response for a model    

---

## ✅ CORS Setup & API Security

### 🎯 Learning Topics
- What is CORS and why it matters in full-stack apps    
- Setting up Laravel CORS (barryvdh/laravel-cors or Laravel built-in CORS)    
- API token protection (sanctum or passport basics)    
- CSRF & API token handling for secure communication    

### 🧩 Mini Tasks
- Setup CORS to allow only React frontend requests    
- Add basic token-based protection to test a secure route    
- Test restricted route access without token    

---

## ✅ React API Integration

### 🎯 Learning Topics
- Using `fetch()` / `axios` to make API calls    
- GET/POST/PUT/DELETE requests    
- Submitting forms to the backend    
- Storing and displaying fetched data    

### 🧩 Mini Tasks
- Create a React form and submit to Laravel backend    
- Fetch blog post data from Laravel API and display it in React    
- Use state to manage form and API data    

---

## ✅ Authentication Flow (React + Laravel)

### 🎯 Learning Topics
- Login/Register API with Laravel Sanctum    
- Token handling and storing auth state in React    
- Protecting frontend routes based on login status    
- Logout functionality and session/token clearing    

### 🧩 Mini Tasks
- Build React login and register forms    
- Handle successful/failed login with appropriate alerts    
- Show dashboard only if user is authenticated    

---

## ✅ Full Stack Database Integration

### 🎯 Learning Topics
- Laravel Eloquent model for working with DB    
- React fetching and updating data via Laravel APIs    
- CRUD operations: create/read/update/delete from UI to DB    
- Error handling for missing records, invalid data    

### 🧩 Mini Tasks:
- React form → Laravel POST → Store in DB    
- Fetch data from DB and display in React table    
- Update/delete DB records from frontend UI    

---

## ✅ Final Project — Full Stack Blog App

### 🎯 Objectives
- Build a full-stack blog app with **React frontend** and **Laravel API backend**    
- Integrate database using **Laravel Eloquent + MySQL**    
- Implement secure **auth** and **CRUD** flows    

### 🧩 Project Tasks:
- User login/register with Laravel Sanctum    
- Auth-protected blog post CRUD (Create, Read, Update, Delete)    
- React dashboard to manage blog posts    
- Connected database for real-time data    
- Error handling & alerts in UI    
- Push to GitHub and deploy frontend/backend if possible

---