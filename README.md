<div align="center">

# Employee Task Tracker

### Enterprise-Grade Employee & Project Management Platform

Manage employees, projects, tasks, deadlines, and team collaboration from a single centralized dashboard.

---

![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-green?style=for-the-badge)
![React](https://img.shields.io/badge/React-19-blue?style=for-the-badge)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue?style=for-the-badge)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-blue?style=for-the-badge)
![JWT](https://img.shields.io/badge/JWT-Secure_Auth-red?style=for-the-badge)

---

###  Built to Learn Real-World Software Engineering

From System Design → Database Design → Backend APIs → Frontend Development → Deployment

</div>

---

# Table of Contents

* Overview
* Problem Statement
* Key Features
* Architecture
* Tech Stack
* Database Design
* System Modules
* API Design
* Project Structure
* Scalability Plan
* Screenshots
* Setup Guide
* Roadmap
* Learning Outcomes

---

# Overview

Employee Task Tracker is a full-stack enterprise productivity platform that helps organizations manage:

✅ Employees

✅ Projects

✅ Tasks

✅ Team Collaboration

✅ Notifications

✅ Productivity Reports

The system follows a **Modular Monolith Architecture**, making it easy to scale into microservices in the future.

---

# Why This Project?

Most organizations struggle with:

* Tasks managed through WhatsApp
* Lack of project visibility
* Missed deadlines
* No employee productivity tracking
* No centralized communication

This platform solves those challenges by providing a centralized workspace for managers and employees.

---

#  Application Flow
![Application Flow](./docs/application-flow.png)

---

# Features

## Authentication & Authorization

* Secure JWT Authentication
* Login & Logout
* Role-Based Access Control (RBAC)
* Protected APIs
* Protected Frontend Routes

---

##  Employee Management

* Add Employee
* Update Employee
* Delete Employee
* Department Assignment
* Role Assignment
* Employee Directory

---

## Project Management

* Create Projects
* Manage Project Members
* Track Project Status
* Project Timeline

---

## Task Management

* Create Tasks
* Assign Tasks
* Set Priority
* Due Date Tracking
* Status Updates
* Task History

---

## Collaboration

* Task Comments
* Activity Timeline
* Team Communication

---

## Reporting

* Employee Productivity
* Task Completion Rate
* Project Progress
* Pending vs Completed Tasks

---

# High-Level Architecture

![Architecture Diagram](./docs/hld.png)

---

## Architecture Pattern

```text
Modular Monolith
```

Benefits:

* Simple deployment
* Easy maintenance
* Fast development
* Future microservice migration

---

# 🔄 System Flow

```text
Users
 │
 ▼
React Frontend
 │
 ▼
REST APIs
 │
 ▼
Spring Boot Backend
 │
 ▼
PostgreSQL Database
```

---

# 🧩 Backend Modules

```text
Auth Module
Employee Module
Project Module
Task Module
Comment Module
Notification Module
Report Module
```

Each module follows:

```text
Controller
    │
    ▼
Service
    │
    ▼
Repository
    │
    ▼
Database
```

---

# 🛠️ Technology Stack

## Frontend

| Technology      | Purpose           |
| --------------- | ----------------- |
| React           | UI Development    |
| TypeScript      | Type Safety       |
| Tailwind CSS    | Styling           |
| ShadCN UI       | Component Library |
| TanStack Query  | Data Fetching     |
| React Hook Form | Form Handling     |
| Zod             | Validation        |

---

## Backend

| Technology      | Purpose               |
| --------------- | --------------------- |
| Java            | Programming Language  |
| Spring Boot     | Backend Framework     |
| Spring Security | Authentication        |
| JWT             | Authorization         |
| Hibernate       | ORM                   |
| Maven           | Dependency Management |

---

## Database

| Technology | Purpose             |
| ---------- | ------------------- |
| PostgreSQL | Relational Database |

---

# 🗄️ Database Design

## Core Entities

```text
Department
Role
Employee
Project
ProjectMember
Task
Comment
Notification
```

---

## Entity Relationship Diagram

![ER Diagram](./docs/er-diagram.png)

---

# 🔄 Task Lifecycle

```text
┌──────────┐
│  TO DO   │
└────┬─────┘
     │
     ▼
┌──────────┐
│IN PROGRESS│
└────┬─────┘
     │
     ▼
┌──────────┐
│ REVIEW   │
└────┬─────┘
     │
     ▼
┌──────────┐
│  DONE    │
└──────────┘
```

---

# 📂 Project Structure

```bash
employee-task-tracker
│
├── docs
│   ├── hld.png
│   ├── er-diagram.png
│   ├── dashboard.png
│
├── frontend
│
├── backend
│
└── README.md
```

---

# 🌐 API Design

## Authentication

```http
POST /api/auth/register
POST /api/auth/login
GET  /api/auth/me
POST /api/auth/logout
```

## Employees

```http
GET    /api/employees
POST   /api/employees
PUT    /api/employees/{id}
DELETE /api/employees/{id}
```

## Projects

```http
GET    /api/projects
POST   /api/projects
PUT    /api/projects/{id}
DELETE /api/projects/{id}
```

## Tasks

```http
GET    /api/tasks
POST   /api/tasks
PUT    /api/tasks/{id}
DELETE /api/tasks/{id}
```

---

# 📸 Screenshots

## Dashboard

![Dashboard](./docs/dashboard.png)

---

## Task Board

![Task Board](./docs/task-board.png)

---

## Project Details

![Project Details](./docs/project-details.png)

---

# 🚀 Future Scalability

```text
Current Architecture
        │
        ▼
 Modular Monolith
        │
        ▼
 Add Redis Cache
        │
        ▼
 Add RabbitMQ
        │
        ▼
 Add AWS S3
        │
        ▼
 Microservices
        │
        ▼
 Kubernetes Deployment
```

---

# 🎯 Development Roadmap

## Phase 1

* Authentication
* Employee Management
* Project Management

## Phase 2

* Task Management
* Comments
* Notifications

## Phase 3

* Reports
* Analytics
* Dashboard

## Phase 4

* Kanban Board
* Time Tracking
* Leave Management

## Phase 5

* Redis
* RabbitMQ
* AWS S3

---

# 📚 Learning Outcomes

This project demonstrates:

* System Design
* HLD & LLD Design
* Database Modeling
* REST API Development
* JWT Authentication
* RBAC Authorization
* Full Stack Development
* Clean Architecture
* Scalable Backend Design
* Enterprise Application Development

---

# ⚡ Local Setup

## Frontend

```bash
cd frontend

npm install

npm run dev
```

## Backend

```bash
cd backend

./mvnw spring-boot:run
```

---

# 👨‍💻 Author

### Siddhi Singh Rathor

Full Stack Developer | Java | Spring Boot | React | Cloud Computing

---

<div align="center">

⭐ Star this repository if you found it useful.

🚀 Built with the goal of learning real-world software engineering.

</div>
