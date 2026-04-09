# 🍽️ E-Mensa — University Canteen Web Application

**Author:** Malek Bouaziz · Ahmed Mehdi Amar
**Course:** Web Development · Praktikum
**Language:** PHP 8.2 · MySQL · Blade Templating

A full-stack web application for a university canteen. Users can browse
daily dishes, log in with their account, and view personalized content.
Built with a custom MVC framework and Blade templating engine.

---

## ⚙️ Features

- Browse and display canteen dishes from a MySQL database
- User authentication with SHA-1 + salt hashing and PHP sessions
- Login / logout with session management
- Custom front controller and URL router
- Blade templating with layouts and reusable views
- Prepared statements (mysqli) for SQL injection prevention
- Monolog logging for requests and errors

---

## 🗂️ Project Structure
├── config/          # Database connection
├── controllers/     # HomeController, AnmeldungController, AbmeldungController
├── models/          # SQL functions: benutzer, gericht, kategorie
├── views/           # Blade templates (home, login, layouts)
├── routes/web.php   # URL → Controller mappings
├── public/
│   ├── index.php    # Front controller + router entry point
│   ├── css/         # Custom styles
│   └── img/         # Dish images and logo
└── composer.json    # Dependencies (BladeOne, Monolog)

---

## 🚀 Getting Started

**Requirements:** PHP 8.2+, MySQL, Composer
```bash
composer install
php -S localhost:8000 -t public
```

Then open `http://localhost:8000` in your browser.


---

## 🧠 Concepts

- MVC pattern with custom routing (no framework)
- Blade templating via BladeOne library
- Secure login with hashed passwords and PHP sessions
- Parameterized SQL queries with mysqli
- Monolog structured logging
