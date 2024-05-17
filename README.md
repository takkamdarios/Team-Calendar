
# Team Calendar

## Introduction

Team Calendar is a web application designed to help users create, view, and manage events efficiently. The app supports two types of users: administrators and regular users. Administrators have full control over events, including the ability to create, view, update, and delete them. Regular users, on the other hand, can only view events. The application interacts with the database through a RESTful API, secured with JWT tokens, and provides a web interface for user interaction.

## Prerequisites

- Docker
- Docker Compose

## Dockerized Applications

### Database

The application uses MariaDB as its database. A Dockerfile located in the `db` directory is used to build a Docker image for MariaDB.

### API

The API service typically operates on port 3000. A Dockerfile in the `api` directory builds the Docker image for the API. When running in Docker, the API can be accessed at [http://localhost:3000](http://localhost:3000), and the API documentation is available at [http://localhost:3000/api](http://localhost:3000/api).

### Web

The frontend is developed using ReactJS. The Dockerfile in the `web` directory is used to build the Docker image for the web application. The web app runs at [http://localhost:3002](http://localhost:3002) when running in Docker.

## Running the Applications

To start all the applications, navigate to the project's root directory and execute the following command:

\`\`\`bash
docker-compose up
\`\`\`

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
