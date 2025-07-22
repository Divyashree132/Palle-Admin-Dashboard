# 🧩 Palle Admin Dashboard

The **Palle Admin Dashboard** is a Django-based web application designed with **Role-Based Access Control (RBAC)**. It allows management of employees and students through two defined user roles: **Admin** and **Sales**. The application focuses on user-specific access, CRUD functionality, and secure data handling using Django and MySQL.

---

## 📌 Project Overview

This project provides a platform where **Admins** have full control over the system, including adding, updating, and deleting both students and employees. **Sales users**, on the other hand, can only add new students and view the student list. The application dynamically adapts the dashboard based on the logged-in user’s role.

---

## 🧠 Key Features

- The system implements Django's authentication system with a custom role-based redirect after login.
- Admin users can access a complete dashboard with options to manage employees and students.
- Sales users are given limited access and can only perform student creation and view operations.
- Each student is assigned using the `added_by` field, which is automatically set for sales users or selectable for admin users.
- Django's messaging framework is used to show success or error messages after user actions.

---

## 🔐 Security Highlights

- Role-based access control ensures that only authorized users can access or modify specific data.
- All POST requests are protected with CSRF tokens to prevent cross-site request forgery.
- Fields like `added_by` are securely managed to prevent unauthorized modifications.
- Sessions are managed effectively to control login and logout behavior across the application.

---

## 💻 Technical Overview

- The backend is developed using **Python** and **Django**, utilizing **Function-Based Views (FBVs)** for precise control.
- **Django ORM** is used for all database interactions, such as `.filter()`, `.get()`, `.create()`, and `.update()`.
- **ModelForms** are used to simplify form creation and validation.
- The frontend is styled using **Django Templates**, **Bootstrap**, and custom CSS.
- **MySQL** is used as the database, with a normalized schema for better data integrity.

---

## ✅ Summary of Functionality

- Admin users have full permissions to manage both employees and students.
- Sales users can add and view students but cannot modify or delete records.
- The application shows different dashboard options based on user roles.
- All views are protected with Django’s built-in user system.
- The admin panel is extended for backend data management using Django’s admin interface.]


> This project was built as part of my hands-on training in full-stack web development and demonstrates my skills in Django, database design, and secure web application development.
