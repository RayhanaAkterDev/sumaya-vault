# 🗄️ Phase 5: Database Management (MySQL + Laravel ORM)

> **🎯 Goal:** Master **MySQL** fundamentals, learn advanced **Eloquent ORM**, and integrate relational data handling into Laravel apps with **optimization and security**.
> ⏳ **Suggested Duration:** 1 Dec 2025 → 31 Dec 2025 (1 month)

---

## ✅ MySQL Fundamentals

### 🎯 Learning Topics
- MySQL database structure: databases, tables, columns    
- Data types, primary keys, indexes    
- Basic CRUD queries: `SELECT`, `INSERT`, `UPDATE`, `DELETE`    
- Querying with `WHERE`, `LIKE`, `ORDER BY`, `LIMIT`, etc.    
- SQL Joins: `INNER JOIN`, `LEFT JOIN`    

### 🧩 Mini Tasks
- Create a MySQL table for `users` and `posts`    
- Write queries to insert, update, and delete rows    
- Practice joining `users` and `posts` to show user-post info    

---

## ✅ Laravel Eloquent ORM (Advanced)

### 🎯 Learning Topics
- Model creation and structure    
- Querying with Eloquent: `where()`, `orderBy()`, `first()`, `pluck()`, etc.    
- Mass assignment and `$fillable`    
- Soft deletes and timestamps    
- Eloquent collections and helper methods    

### 🧩 Mini Tasks
- Create `User` and `Post` models    
- Fetch and display a list of users with their latest posts    
- Use Eloquent methods to filter data (e.g., top 5 posts by views)    

---

## ✅ Database Relationships

### 🎯 Learning Topics
- One-to-Many: `User` → `Posts`    
- Many-to-Many: `Post` ↔ `Tag`    
- HasOne, HasMany, BelongsTo, BelongsToMany    
- Accessing related data with `with()` and `load()`    
- Querying relationships and eager loading    

### 🧩 Mini Tasks
- Create a `Tag` model and set up many-to-many with `Post`    
- Fetch posts with all related tags and display    
- Eager load user data when fetching posts (`Post::with('user')`)    

---

## ✅ Migrations, Seeders & Factories

### 🎯 Learning Topics
- Creating and running migrations    
- Database seeding with dummy data    
- Using factories to generate bulk data for testing    
- Relationships within factories (e.g., post belongs to user)    

### 🧩 Mini Tasks
- Create migrations for users, posts, and tags tables    
- Use seeders to insert 10 users and 50 posts    
- Generate factories for posts with fake content and tags    

---

## ✅ Query Optimization & Security

### 🎯 Learning Topics
- Indexing for faster queries    
- Avoiding N+1 query problem (use eager loading)    
- Parameterized queries (SQL injection prevention)    
- Using Laravel’s query logs and performance tips    
- Caching (optional intro via Laravel Cache)    

### 🧩 Mini Tasks
- Optimize a query using indexing and `with()`    
- Protect a raw query with parameter binding    
- Measure and compare query performance using Laravel Debugbar    

---

## ✅ Final Project — Database-Centric Blog

### 🎯 Objectives
- Build a Laravel blog app focused on robust **database structure**, **relationships**, and **performance**
- Implement **real-world data interaction** via MySQL    

### 🧩 Project Tasks
- Models: User, Post, Comment, Tag    
- Relationships:    
    - User → Posts (One-to-Many)        
    - Post ↔ Tags (Many-to-Many)        
    - Post → Comments (One-to-Many)        
- Use seeders and factories to simulate a working blog    
- Optimize post-fetching with eager loading    
- Secure inputs and protect against SQL injection    
- Backup database and export via `.sql` (optional advanced task)

---