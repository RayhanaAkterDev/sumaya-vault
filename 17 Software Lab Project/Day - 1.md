# 🗓 Day 1 – HMS Setup & GitHub

## Step 1: Install Required Tools

Make sure you have all tools installed on your system:

- [x] Git → version control  
- [x] Node.js & npm → React frontend  
- [x] PHP & Composer → Laravel backend  
- [x] MySQL → Database  

Verify installation:

```bash
git --version
node -v
npm -v
php -v
composer -v
mysql --version
```

---

## Step 2: Create GitHub Repository

- [x] Go to [GitHub](https://github.com) and sign in  
- [x] Click **New Repository**  
- [x] Repository name: `hospital-management-system`  
- [x] Add description: “Hospital Management System – Semester Project”  
- [x] Optional: Initialize with README  
- [x] Clone repository locally:

```bash
git clone https://github.com/<your-username>/hospital-management-system.git
cd hospital-management-system
```

---

## Step 3: Create Project Folder Structure

Inside the cloned repo, create main project folders:

```bash
mkdir backend frontend database
```

Folder purpose:

- `backend/` → Laravel project  
- `frontend/` → React project  
- `database/` → Optional: SQL dumps / migration backups  

Expected folder structure:

```text
hospital-management-system/
├─ backend/
├─ frontend/
├─ database/
└─ README.md
```

---

## Step 4: Initialize Git & Make First Commit

- [ ] Stage all files:

```bash
git add .
```

- [ ] Commit changes:

```bash
git commit -m "init project structure with backend, frontend, database folders"
```

- [ ] Push to GitHub:

```bash
git push origin main
```

---

## Step 5: Optional Live Demo (Frontend)

- [ ] Deploy a simple React “Home Page” to **Vercel** or **Netlify** as a placeholder.  
- [ ] Shows project is live even before backend is ready.

---

## ✅ Day 1 Goals

- [x] Install all tools  
- [x] GitHub repository created  
- [ ] Project folder structure ready  
- [ ] First commit done  
- [ ] Optional live placeholder page deployed
