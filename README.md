## 🚌 Bus Booking System — CodeIgniter PHP Project

A simple **Bus Booking System** built using the **CodeIgniter PHP framework**. This project lets users view available buses, book tickets, and manage bookings through a clean web interface.

---

### 📁 Project Structure

Your project folders:

```
/
├── application/    # Your CodeIgniter application (controllers, models, views)
├── system/         # CodeIgniter core framework files
├── assets/         # CSS, JS, images, etc.
├── database/       # SQL dumps or migrations (optional)
├── uploads/        # Uploaded files (if any)
├── Documentation/  # Project docs (if included)
├── index.php       # Front controller
├── .DS_Store       # System file (macOS, ignore)
├── img.png         # Project image/logo (optional)
```

---

### ✅ Features

* View available buses & routes
* Book bus tickets online
* Track bookings
* Admin panel to manage buses (if implemented)
* MVC structure using CodeIgniter framework

---

### ⚙️ Requirements

* **PHP** (7.x or above recommended)
* **MySQL** / MariaDB
* **Apache** server (XAMPP, WAMP, LAMP, MAMP)
* Browser (Chrome, Firefox, etc.)

---

### ⚡ How to Run

1️⃣ **Place Project Folder**

Copy the entire project folder into your web server’s root:

* XAMPP → `C:\xampp\htdocs\YourProjectFolder`
* WAMP → `C:\wamp\www\YourProjectFolder`
* LAMP → `/var/www/html/YourProjectFolder`

---

2️⃣ **Create Database**

1. Open **phpMyAdmin** or MySQL CLI
2. Create a database:

   ```sql
   CREATE DATABASE bus_booking;
   ```
3. Import your SQL file (if any) located in the `/database/` folder:

   ```
   Import bus_booking.sql
   ```

---

3️⃣ **Configure Database**

Open `application/config/database.php` and update:

```php
'hostname' => 'localhost',
'username' => 'root',
'password' => '',
'database' => 'bus_booking',
```

---

4️⃣ **Set Base URL**

In `application/config/config.php`, update:

```php
$config['base_url'] = 'http://localhost/YourProjectFolder/';
```

---

5️⃣ **Set Default Controller**

Open `application/config/routes.php`:

```php
$route['default_controller'] = 'Welcome'; // or your main controller
```

---

6️⃣ **Start Apache & MySQL**

Use XAMPP/WAMP/LAMP to start **Apache** & **MySQL** services.

---

7️⃣ **Run the Project**

Open your browser:

```
http://localhost/YourProjectFolder/
```

✅ Your CodeIgniter Bus Booking System is ready to use!

---

### 🚦 Troubleshooting

* **404 Error?**

  * Make sure `default_controller` is correct.
  * Check `.htaccess` and `mod_rewrite` is enabled (for clean URLs).

* **Database Connection Error?**

  * Verify credentials in `database.php`.
  * Make sure MySQL is running.

---

### 📌 Important

* Always validate & sanitize user input.
* Use secure password hashing (`bcrypt`).
* Store `uploads/` securely (if you handle file uploads).
* For production, hide `index.php` using `.htaccess`.

---

### 🗂️ Credits

* Built with **CodeIgniter PHP Framework**.
* Author: *Jayasimma D*
* License: *MIT*

---
