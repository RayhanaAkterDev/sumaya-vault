### 🔹 Main Branch

- `main` → stable, production-ready code.   

---

### 🔹 Setup Branches

- `frontend/setup` → initial React project setup, install basic packages.   
- `backend/setup` → initial Laravel project setup, install basic packages.

---

### 🔹 Feature Branches

#### Frontend

- `frontend/homeui` → homepage feature (overall branch for homepage).    
    - `frontend/homeui-navbar` → sub-feature for navbar section. 
    - `frontend/homeui-hero` → sub-feature for hero banner section.
    - `frontend/homeui-services` → sub-feature for services section (big section with multiple pages).
    - `frontend/homeui-contact` → sub-feature for contact section.
- `frontend/global-styles` → global CSS/SCSS changes, themes, layout styles.

---

#### Backend

- `backend/user-role` → user role management system.
- `backend/intervention-image` → image processing feature.
- `backend/api-auth` → API authentication module.

---

### 🔹 Key Notes

- **Setup branches** → merged into main, then deleted.
- **Feature branches** → branch off main (or setup if not merged yet).
- **Sub-feature branches** → only for big sections, branch off the main feature branch.

- After work is finished → merge sub-feature → feature → main.