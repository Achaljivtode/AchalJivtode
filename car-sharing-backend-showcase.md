# 🚗 Car Sharing System – Backend Showcase (Django + DRF)

This is a **backend-focused personal showcase** of the Car Sharing System I built as part of a group project.  
The **entire backend** (models, APIs, authentication, admin panel) was developed by me.

🔗 **Project Repository**: [Car Sharing System – Fullstack](https://github.com/Achaljivtode/Car-Sharing-System)

---

## 🧑‍💻 My Role – Backend Developer

I was solely responsible for designing and developing the backend logic and REST API. My contributions include:

- ✅ Designing the database schema and models
- ✅ Creating secure and scalable APIs using Django REST Framework
- ✅ Implementing JWT Authentication and Password Reset using SimpleJWT
- ✅ Customizing Django Admin for better model management
- ✅ Building admin-only features (e.g., feature table access control)
- ✅ Integrating the backend with the frontend (React)

---

## 🏗️ Backend Architecture

### 🔹 Models I Created
- `CustomUser` (with roles: admin and user)
- `Car` – car listings with price, image, etc.
- `CarBook` – booking a car
- `Enquiry` – user queries
- `Feature` – only admins can access

### 🔹 Authentication
- JWT Authentication via SimpleJWT
- Token Refresh system
- Password Reset endpoints

### 🔹 Admin Panel
- Customized Django Admin with filters, search, and inline displays
- Admin-only access to key models like `Feature`

---

## ⚙️ Tech Stack

| Layer        | Tech                          |
|--------------|-------------------------------|
| Backend      | Django, Django REST Framework |
| Auth         | SimpleJWT (JWT Tokens)        |
| Database     | MySQL                         |
| Admin Panel  | Django Admin                  |
| Frontend     | React (handled by teammate)   |

---

## 📸 Screenshots

> These show how the backend powers the UI built by the frontend dev

| Page              | Screenshot Path |
|-------------------|------------------|
| Home Page         | ![Home](frontend/Resources/screenshots/homepage.png) |
| Register Page     | ![Register Page](frontend/Resources/screenshots/register_page.png) |
| Login Page        | ![Login Page](frontend/Resources/screenshots/login_page.png) |
| Contact Page      | ![Contact Page](frontend/Resources/screenshots/contact_page.png)|
| Admin Dashboard   | ![Customer Dashboard](frontend/Resources/screenshots/customer_dashboard.png)|
| Customer Dashboard| ![Admin Dashboard](frontend/Resources/screenshots/admin_dashboard.png)|
| Profile Page      | ![Profile Page](frontend/Resources/screenshots/profile_page.png)|

---

## 📂 Project Structure

```bash
car-sharing-system/
├── backend/
│   ├── app/
│   ├── backend/
│   ├── media/         
│   ├── manage.py
├── frontend/             # Built in React (teammate)
│   ├── src/
│   ├── public/


🚀 Local Setup
bash

# Clone project
git clone https://github.com/Achaljivtode/Car-Sharing-System.git
cd Car-Sharing-System

# Backend setup
python -m venv env
# On Windows: env\Scripts\activate
pip install -r requirements.txt

# MySQL config in settings.py

# Use environment variables for production

# Migrate and run
python manage.py makemigrations
python manage.py migrate
python manage.py runserver

📌 API Authentication Endpoints
Action	         Endpoint
Register	       /api/register/
Login (Token)	   /api/token/
Refresh Token	   /api/token/refresh/
Password Reset	 Supported via DRF

🔗 Full Project Repo
https://github.com/Achaljivtode/Car-Sharing-System

