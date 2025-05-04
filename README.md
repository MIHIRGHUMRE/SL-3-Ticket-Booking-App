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

![Screenshot 2025-04-25 165624](https://github.com/user-attachments/assets/a8a9bf1d-df06-4d43-8bb7-2e89f18b7224)
![Screenshot 2025-04-25 165818](https://github.com/user-attachments/assets/ee61df26-c229-40fb-9e94-566fe784e5cc)
![Screenshot 2025-04-25 170240](https://github.com/user-attachments/assets/470b4e96-8203-4b4a-9e60-8bf0a289ac1e)
![Screenshot 2025-04-25 170509](https://github.com/user-attachments/assets/d088f059-725b-4b4a-8584-1f084915edd0)
![Screenshot 2025-04-25 170525](https://github.com/user-attachments/assets/3c4a546d-09d1-4392-acbd-e210c8c23518)
![Screenshot 2025-04-25 170538](https://github.com/user-attachments/assets/13e21fe6-df90-4d1c-852c-cf5f2fc26afc)
![Screenshot 2025-04-25 170556](https://github.com/user-attachments/assets/9f69b1c0-a98b-4ce9-ae96-d1f105322f2a)
![Screenshot 2025-04-25 165536](https://github.com/user-attachments/assets/a9a50b5c-9763-4d20-93a0-115ef33e6e31)


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
