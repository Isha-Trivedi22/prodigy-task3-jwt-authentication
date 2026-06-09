# Task 3 - JWT Authentication and Authorization

## Description

This project demonstrates JWT-based Authentication and Authorization using Node.js, Express.js, MongoDB Atlas, Mongoose, bcryptjs, and JSON Web Tokens.

## Features

* User Registration
* User Login
* Password Hashing using bcryptjs
* JWT Token Generation
* Protected Routes
* MongoDB Atlas Integration
* Environment Variables using dotenv

## Technologies Used

* Node.js
* Express.js
* MongoDB Atlas
* Mongoose
* bcryptjs
* JSON Web Token (JWT)
* dotenv

## API Endpoints

### Register User

POST /api/auth/register

Request:

```json
{
  "name": "Isha",
  "email": "isha.task3@gmail.com",
  "password": "123456"
}
```

### Login User

POST /api/auth/login

Request:

```json
{
  "email": "isha.task3@gmail.com",
  "password": "123456"
}
```

Response:

```json
{
  "token": "JWT_TOKEN"
}
```

### Protected Route

GET /api/auth/profile

Headers:

```text
Authorization: Bearer JWT_TOKEN
```

Response:

```json
{
  "message": "Protected Route Accessed",
  "userId": "USER_ID"
}
```

## Project Structure

```
Task-3-JWT-Authentication
│
├── middleware
│   └── auth.js
│
├── models
│   └── User.js
│
├── routes
│   └── authRoutes.js
│
├── .env
├── .gitignore
├── package.json
├── server.js
```

## Learning Outcomes

* Authentication vs Authorization
* Password Hashing
* JWT Token Generation and Verification
* Route Protection using Middleware
* MongoDB Atlas Integration
* Environment Variable Management

## Author

Isha Trivedi
