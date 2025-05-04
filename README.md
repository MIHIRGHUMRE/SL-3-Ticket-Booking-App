# SL-3-Ticket-Booking-App
# 🎟️ Ticket Booking System

A web-based ticket booking system for managing shows, seat selections, and user bookings. Built with Django, Dockerized for easy deployment, and integrated with Jenkins for CI/CD automation.

---

## 📌 Project Overview

This project includes:

- Custom Django admin panel (no default Django Admin)

- User management and authentication

- PostgreSQL database integration

- Dockerized environment for local development

- Optional Jenkins support for CI/CD (extendable)

- Pre-built setup fix for PostgreSQL connection issues

---

## 🛠️ Tech Stack Used

- **Backend**: Django (Python)
- **Frontend**: HTML, CSS (Bootstrap)
- **Database**: PostgreSQL
- **Containerization**: Docker, Docker Compose
- **CI/CD**: Jenkins
- **Authentication**: Django’s built-in auth system
- **Others**: Gunicorn (for production), Whitenoise (for static files)

---

## ⚙️ Setup & Run Instructions

### 🔧 Prerequisites
- Docker
- Docker Compose
- Git

### 🚀 Quickstart

```bash
# Clone the repository
git clone https://github.com/tailormst/SL-3-Ticket_Booking_APP
cd ticket_booking_system

# Build and run the containers
docker-compose up --build

# Create superuser (optional)
docker-compose exec web python manage.py createsuperuser

# Access the app
Visit http://localhost:8000
```


# 📸 Screenshots

![Screenshot 2025-04-25 165624](https://github.com/user-attachments/assets/425d9a71-2a8a-4c25-8018-e569023955d9)
![Screenshot 2025-04-25 165818](https://github.com/user-attachments/assets/20737093-0a6a-473d-b336-a94234c9270a)
![Screenshot 2025-04-25 170240](https://github.com/user-attachments/assets/28895482-196f-4805-a55a-fb88d8b0c8a5)
![Screenshot 2025-04-25 170509](https://github.com/user-attachments/assets/da76b97f-0bca-4458-8e1b-9df0a00a48b2)
![Screenshot 2025-04-25 170525](https://github.com/user-attachments/assets/9d4253f3-4956-4f17-944b-ee5c8dcde2b3)
![Screenshot 2025-04-25 170538](https://github.com/user-attachments/assets/5ebd4a6b-cf3e-41aa-8772-fc38d8d356f7)
![Screenshot 2025-04-25 170556](https://github.com/user-attachments/assets/326dfd1f-7fb9-49cc-aef0-2bac7de71bb0)
![Screenshot 2025-04-25 165536](https://github.com/user-attachments/assets/d4833640-a913-46a4-98c8-bda6f7d49d90)


# 🐳 Docker Usage
Dockerfile and docker-compose.yml are configured to:

Run the Django app with Gunicorn

Use a separate PostgreSQL container

Automatically collect static files

To restart the service:

docker-compose down
docker-compose up --build

# ⚙️ Jenkins Usage
If you use Jenkins:

Add Jenkinsfile with pipeline stages like:

Pull code

Build image

Run tests

Deploy to Docker

Make sure:

Jenkins has Docker installed

Your pipeline is set to trigger on Git pushes

# 📄 License
This project is licensed under the MIT License.
