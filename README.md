<h1 align="center">🗓️ Team Calendar</h1>
<h3 align="center">A Web Application for Efficient Event Management</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white" alt="NestJS">
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white" alt="JavaScript">
  <img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="MariaDB">
</p>

---

## 🌟 Introduction

**Team Calendar** is a web application designed to help users create, view, and manage events efficiently. The app supports two types of users:

- **Administrators**: Full control over events (create, view, update, delete)
- **Regular Users**: View events only

The application interacts with the database through a RESTful API, secured with JWT tokens, and provides a web interface for user interaction.

---

## 🛠 Prerequisites

- Docker
- Docker Compose

---

## 📦 Dockerized Applications

### Database

The application uses **MariaDB** as its database. A Dockerfile located in the `db` directory is used to build a Docker image for MariaDB.

### API

The API service typically operates on port 3000. A Dockerfile in the `api` directory builds the Docker image for the API. When running in Docker, the API can be accessed at [http://localhost:3000](http://localhost:3000), and the API documentation is available at [http://localhost:3000/api](http://localhost:3000/api).

### Web

The frontend is developed using **Next.js** and **JavaScript**. The Dockerfile in the `web` directory is used to build the Docker image for the web application. The web app runs at [http://localhost:3002](http://localhost:3002) when running in Docker.

---

## 🚀 Running the Applications

To start all the applications, navigate to the project's root directory and execute the following command:

```bash
docker-compose up



### Administrator Credentials

- **Email:** admin@email.com
- **Name:** Administrator
- **Password:** Admin@Password1
- **Role ID:** 1

### Important Information

- When creating a user, enter `1` for admin and `2` for regular user in the Role field.
- Password requirements:
  - At least one uppercase letter
  - At least one lowercase letter
  - At least one number
  - At least one special character
  - Minimum of 8 characters
- The email must be a valid email address.
