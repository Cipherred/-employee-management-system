# -employee-management-system
اكتبي هذا الوصف:  **Employee Management System built with Spring Boot, REST APIs, JPA/Hibernate, DTOs, Validation, and Spring Security with role-based access control.**
# Employee Management System

A secure full-stack Employee Management System built with **Java, Spring Boot, Spring Security, JWT, Spring Data JPA, PostgreSQL, and JavaScript**.

The system provides employee management, leave requests, salary advance requests, authentication, role-based authorization, employee-level data isolation, and administrative approval workflows.

## Tech Stack

- **Backend:** Java, Spring Boot
- **Security:** Spring Security, JWT, BCrypt
- **Database:** PostgreSQL
- **ORM:** Spring Data JPA / Hibernate
- **Frontend:** HTML, CSS, JavaScript
- **API Testing:** Postman
- **Architecture:** Controller → Service → Repository

## Key Features

- JWT-based authentication
- Role-Based Access Control (ADMIN / EMPLOYEE)
- Employee-level data isolation
- Employee management
- Leave request management
- Salary advance request management
- Admin approval/rejection workflows
- RESTful CRUD APIs
- DTO-based request/response handling
- Server-side validation
- Centralized exception handling
- Relational database mapping
- Secure authenticated API communication

## Quick Overview

### ADMIN

Administrators can:

- View and manage employees
- Add new employees
- View all leave requests
- Approve or reject leave requests
- View all salary advance requests
- Approve or reject salary advance requests

### EMPLOYEE

Employees can:

- Log in securely
- Submit leave requests
- Submit salary advance requests
- View their own requests
- Track request status

Employees cannot access another employee's requests.

## Screenshots

### Login

![Login](screenshots/login.png)

### Admin Dashboard

![Admin Dashboard](screenshots/admin-dashboard.png)

### Employee Management

![Employee Management](screenshots/employee-management.png)

### Leave Requests

![Leave Requests](screenshots/leave-requests.png)

### Salary Advance Requests

![Advance Requests](screenshots/advance-requests.png)

### Employee Dashboard

![Employee Dashboard](screenshots/employee-dashboard.png)

---

# Detailed Documentation

## 1. System Architecture

The backend follows a layered architecture:

```text
Controller
    ↓
Service
    ↓
Repository
    ↓
Database
