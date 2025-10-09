### Add user roll in user table

- open >> HSM project in `vscode` 
- open folder >> folder > file `.env` > copy paste the following code:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=databaseName
DB_USERNAME=root
DB_PASSWORD=
```

- open folder >> backend > database > migration > file `0001_01_01_000000_create_users_table.php` >> add user-roll in the user-table:

```php
$table->enum('role', ['admin', 'doctor', 'assistant', 'patient'])->default('patient');
```

- terminal go to the backend folder and run the command `php artisan migrate`
> it will create the user table in the HSM DB along with the default other tables and user role in user role.

---

### Create New Branch for Adding user-role

- `git checkout -b feature/user-roles`
- `git add .`
- `git commit`

```plaintext
	feat(users): add role enum to users table with default value

- Added ENUM column 'role' with values: admin, doctor, assistant, patient
- Set default role to 'patient'
- Updated .env configuration if needed
```

- `git push -u origin feature/user-roles`

---

### Add detailed project README 

- Go back to the main branch: `git checkout main`
- add a detailed project README on HSM.

---

### Install `Intervention Image` Package

- Open link: image.intervention.io/v3/getting-started/installation
- Copy and run command in project: `composer require intervention/image`
- This package helps in creating image thumbnails

---

### Open the Laravel folder on browser

- run the command: `php artisan serve`
- the command will give a link, open it in browser: `http://127.0.0.1:8000/` or
- go to browser and type: `localhost:8000`
- it will show the default Laravel project interface

---

### Update backend branch names

---

### Create a new branch for React installation and set up the frontend folder

- a new branch name as `frontend/setup` then
- install the following
	- react frontend folder - 
		- `npm create vite@latest frontend`
		- `npm install`
	- react router dom -  `npm install react-router-dom`
	- react hook form - `npm install react-hook-form`
	- react tostify - `npm install react-toastify`
	- react icons - `npm install react-icons`
	- tailwind - `npm install tailwindcss @tailwindcss/vite`

---

### 