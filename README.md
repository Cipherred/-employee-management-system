# Employee Management System

**Employee Management System built with Spring Boot, REST APIs, JPA/Hibernate, DTOs, Validation, and Spring Security with role-based access control.**

A secure full-stack Employee Management System built with **Java, Spring Boot, Spring Security, JWT, Spring Data JPA, Microsoft SQL Server (MSSQL), and JavaScript**.

The system provides employee management, leave requests, salary advance requests, authentication, role-based authorization, employee-level data isolation, and administrative approval workflows.

---

## Tech Stack

- **Backend:** Java, Spring Boot
- **Security:** Spring Security, JWT, BCrypt
- **Database:** Microsoft SQL Server (MSSQL)
- **ORM:** Spring Data JPA / Hibernate
- **Frontend:** HTML, CSS, JavaScript
- **API Testing:** Postman
- **Architecture:** Controller → Service → Repository

---

## Key Features

- JWT-based authentication
- Role-Based Access Control (ADMIN / EMPLOYEE)
- Employee-level data isolation
- Employee management
- Leave request management
- Salary advance request management
- Admin approval and rejection workflows
- RESTful CRUD APIs
- DTO-based request/response handling
- Server-side validation
- Centralized exception handling
- Relational database mapping
- Secure authenticated API communication

---

# Quick Overview

## ADMIN

Administrators can:

- View employees
- Add new employees
- Manage employee information
- View all leave requests
- Approve or reject leave requests
- View all salary advance requests
- Approve or reject salary advance requests

## EMPLOYEE

Employees can:

- Log in securely
- Submit leave requests
- Submit salary advance requests
- View their own requests
- Track request status

Employees cannot access another employee's requests.

---

# Screenshots

## 1. Login

![Login](screenshots/Login.png)

Secure login using employee or administrator credentials.

---

## 2. Admin Dashboard — Employees

![Admin Dashboard - Employees](screenshots/adminDashboard1.png)

The administrator dashboard displays employees in the system and provides access to employee management functions.

---

## 3. Admin Dashboard — Leave Requests

![Admin Dashboard - Leave Requests](screenshots/adminDashboard2.png)

The administrator dashboard displays employee leave requests and allows administrators to review and manage their status.

---

## 4. Admin Dashboard — Salary Advance Requests

![Admin Dashboard - Salary Advance Requests](screenshots/adminDashboard3.png)

The administrator dashboard displays employee salary advance requests and allows administrators to review and manage their status.

---

## 5. Add Employee

![Add Employee](screenshots/adminDashboardAddEmployee.png)

Administrators can create new employee accounts and assign their roles.

---

## 6. Employee Dashboard

![Employee Dashboard](screenshots/EmployeeDashboard1.png)

Employees can view their own requests and track their current status.

---

## 7. Leave Request Form

![Leave Request Form](screenshots/LeaveRequestFillForm.png)

Employees can submit leave requests by providing a start date, end date, and reason.

---

## 8. Leave Request

![Leave Request](screenshots/LeaveRequest.png)

Leave requests display the employee, dates, reason, and current request status.

---

## 9. Salary Advance Request Form

![Salary Advance Request Form](screenshots/AdvnceRequestFillForm.png)

Employees can submit salary advance requests by providing an amount and reason.

---

## 10. Salary Advance Request

![Salary Advance Request](screenshots/AdvanceRequest.png)

Salary advance requests display the employee, requested amount, reason, and current request status.

---

## 11. Input Validation

![Validation Example](screenshots/ValidationExample.png)

The application validates user input before processing requests. For example, email fields must contain a valid email format and advance amounts must be greater than zero.

---

## 12. Exception Handling

![Exception Example](screenshots/ExceptionExample.png)

The application handles invalid requests and displays an appropriate error message when a leave request uses a start date in the past.

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
