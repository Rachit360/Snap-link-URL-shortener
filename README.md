<<<<<<< HEAD
# SnapLink - A URL Shortener

[![Django CI](https://github.com/madhvi-n/snaplink/actions/workflows/django.yml/badge.svg?branch=main)](https://github.com/madhvi-n/snaplink/actions/workflows/django.yml)
[![Python](https://img.shields.io/badge/Python-3.11-blue)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-5.1-brightgreen?style=flat&logo=django&logoColor=white)](https://www.djangoproject.com/)
[![Django Rest Framework](https://img.shields.io/badge/Django_Rest_Framework-3.15-red)](https://www.django-rest-framework.org/)
[![React](https://img.shields.io/badge/React-19-blueviolet)](https://react.dev/)

SnapLink is a **modern, scalable URL shortener** built with **Django (Python) and React (Frontend)**. It allows users to **shorten URLs, track visits, and manage links** via a **REST API & Web Interface**.

## ✨ Features

### 🔗 Core URL Shortening
- Convert long URLs into short, shareable links
- Support for custom vanity URLs (Planned)

### 📊 Analytics & Tracking
- Click Tracking – Monitor total clicks per short URL
- Daily Unique Visitors – Track users based on IP
- Geolocation & Device Data (Future Feature)

### ⏳ Expiration & One-Time Use
- Set Expiration – Define a custom expiry date for short links
- One-Time Use Links – Auto-delete after first visit

### 🔒 User Authentication & Authorization
- JWT-Based Authentication with access_token & refresh_token
- User Registration & Login
- Personalized Dashboard – Users can manage their URLs

### ⚡ Performance & Caching
- Django Cache (Redis) for fast URL redirection
- Database Indexing & Optimization for efficient queries

### 🚀 DevOps & Scalability
- ✅ PostgreSQL Database Integration
- ✅ Rate Limiting for API security (Django Rest Framework)
- 🔜 Dockerized Deployment (Planned)
- 🔜 CI/CD Pipelines with GitHub Actions (Planned)
- 🔜 Error Monitoring with Sentry (Planned)

## 📸 Screenshots

![SnapLink Home](screenshots/image01.png?raw=true "SnapLink Home")

![SnapLink Shorten Url](screenshots/image02.png?raw=true "SnapLink Shorten Url")


## 🛠 Tech Stack

### **Backend:**

- **Python** (Django)
- **Django REST Framework** (DRF)
- **PostgreSQL** (Database)
- **Redis** (Caching)


### **Frontend:**

- **React** (with Vite)
- **Tailwind CSS** (for styling)


## 📦 Installation & Setup

1. Clone the Repository

    ```sh
    git clone https://github.com/madhvi-n/snaplink.git
    cd snaplink
    ```

2. Set up a virtual environment

    ```bash
    python -m venv venv
    source venv/bin/activate  # On macOS/Linux
    venv\Scripts\activate  # On Windows
    ```

3. Install Dependencies

    ```bash
    pip install -r requirements.txt
    ```

4. Set up PostgreSQL database
    ```sh
    sudo -u postgres psql
    CREATE DATABASE snaplink;
    CREATE USER snaplink_user WITH PASSWORD 'yourpassword';
    ALTER ROLE snaplink_user SET client_encoding TO 'utf8';
    ALTER ROLE snaplink_user SET default_transaction_isolation TO 'read committed';
    ALTER ROLE snaplink_user SET timezone TO 'UTC';
    GRANT ALL PRIVILEGES ON DATABASE snaplink TO snaplink_user;
    ```

5. Apply Database Migrations & Create Superuser

    ```bash
    python manage.py migrate
    python manage.py createsuperuser
    ```

6. Run the Development Server

    ```bash
    python manage.py runserver
    ```

    Access at: <http://127.0.0.1:8000>

## Frontend

1. Navigate to the Frontend Folder
    ```sh
    cd frontend/snap_link
    ```

2. Install dependencies

    ```bash
    npm install
    ```

3. Set Backend API URL
    Create a .env file in the frontend root and add:

    ```sh
    VITE_API_URL=http://localhost:8000/api/v1
    ```

4. Start the development server
    ```bash
    npm run dev
    ```


## 📝 API Documentation

The API documentation is available via **Swagger**:

- **Swagger UI:** `http://127.0.0.1:8000/api/swagger/`
- **Redoc:** `http://127.0.0.1:8000/api/redoc/`
- **DRF Browsable API:** `http://127.0.0.1:8000/api/v1/`


## ⚙️ Environment Variables *(Example .env file)*

```ini
SECRET_KEY=django-secret-key
DEBUG=True
BASE_URL=http://localhost:8000
REDIS_URL=your-redis-url
ALLOWED_HOSTS=localhost,127.0.0.1
DB_NAME=snaplink
DB_USER=postgres
DB_PASSWORD=123456
```

# 🚀 Deployment Guide (Coming Soon)
- Dockerization
- CI/CD Pipelines with GitHub Actions
- Production Database Setup

# 🛤 Roadmap & Future Features
### Completed Features
- ✅ Core URL Shortening (short links)
- ✅ Click Tracking (monitor total clicks per URL)
- ✅ Expiration & One-Time Use Links
- ✅ JWT-Based Authentication (access_token & refresh_token)
- ✅ User Registration & Login
- ✅ PostgreSQL Database Integration
- ✅ Rate Limiting for API security

### Upcoming Features
- ⬜ Custom Vanity URLs (personalized short links)
- ⬜ Geolocation & Device Tracking
- ⬜ User Dashboard for managing URLs
- ⬜ Dockerized Deployment
- ⬜ CI/CD Pipelines with GitHub Actions
- ⬜ Error Monitoring with Sentry


### 🎉 Happy Coding! 🚀
=======
# SnapLink-URL-Shortener-Backend-Service
>>>>>>> 5ec76696980736d835fb8c0c449c3205cb9b2f84
