You are a senior full-stack engineer. Build a production-grade Task Management system with clean architecture, scalability, and best practices.

## 🎯 Goal

Create a full-stack Task Tracker application with authentication, offline-first support, and API sync.

---

## 🧱 Tech Stack

### Frontend

* React (Vite)
* TypeScript
* Tailwind CSS
* React Query (TanStack Query)
* Zustand (state management)

### Backend

* Node.js (Express)
* TypeScript
* Prisma ORM

### Database

* PostgreSQL

### Other

* JWT Authentication
* Docker support
* REST API (structured)
* Zod (validation)

---

## 📁 Project Structure

Monorepo style:

/apps
/client
/server
/packages
/types
/utils

---

## 🔐 Authentication

* Register/Login system
* JWT (access + refresh token)
* Password hashing (bcrypt)
* Middleware for protected routes

---

## 🧩 Core Features

### Task System

* Create task
* Update task
* Delete task
* Mark complete
* Add due date
* Add priority (low, medium, high)
* Add description

### Advanced Features

* Pagination
* Filtering (status, priority)
* Search (fuzzy search)
* Sorting

---

## 📡 Offline-first Sync (IMPORTANT)

Implement:

* If API fails:
  → store tasks locally (IndexedDB or localStorage)

* When connection is restored:
  → auto-sync unsynced tasks to server

* Track sync status:

  * pending
  * synced
  * failed

---

## 🗄️ Database Design (Prisma)

User:

* id
* email
* password
* createdAt

Task:

* id
* title
* description
* status
* priority
* dueDate
* userId
* createdAt
* updatedAt

---

## 🔌 API Design

Use REST:

POST   /auth/register
POST   /auth/login

GET    /tasks
POST   /tasks
PUT    /tasks/:id
DELETE /tasks/:id

Support:

* pagination (?page=1&limit=10)
* filtering (?status=completed)
* search (?q=task)

---

## 🧠 Backend Architecture

* Controller layer
* Service layer
* Repository layer
* Middleware (auth, error handling)
* Centralized error handler
* Logging system (Winston or Pino)

---

## 🎨 Frontend Pages

* Login Page
* Register Page
* Dashboard
* Task List Page

---

## ⚡ UI Features

* Optimistic UI updates
* Loading states
* Error handling UI
* Toast notifications

---

## 🧪 Testing

* Backend: Jest
* Frontend: React Testing Library

---

## 🐳 Docker

* Dockerfile for server
* Dockerfile for client
* docker-compose with PostgreSQL

---

## 🔒 Security

* Input validation (Zod)
* Rate limiting
* CORS config
* Helmet

---

## 🚀 Dev Experience

* ESLint + Prettier
* Environment variables (.env)
* API client abstraction
* Reusable hooks

---

## 📦 Bonus Features (if possible)

* Dark mode 🌙
* Drag & drop tasks
* Real-time sync (WebSocket or polling)

---

## 📌 Requirements

* Use clean code principles
* Follow scalable folder structure
* Use TypeScript everywhere
* Write reusable components
* Avoid code duplication
* Write comments where necessary

---

## 📤 Output Format

* Generate full project code step by step
* Start from backend setup → then frontend
* Include commands to run project
* Include environment variables example
* Include DB migration steps

---

Build the project like a real production SaaS starter template.
