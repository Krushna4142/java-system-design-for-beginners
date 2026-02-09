# Day 04 – REST APIs & Request Flow (Quick Notes)

---

## 🔹 What is a REST API?

A **REST API** is a way for a client to communicate with a server using **HTTP requests**.

REST APIs define:

- How requests are sent
- How data is requested or modified
- How responses are returned

📌 REST APIs are the backbone of backend systems.

---

## 🌐 HTTP Methods (Beginner Level)

Common HTTP methods used in REST APIs:

- **GET** → Retrieve data
- **POST** → Create new data
- **PUT** → Update existing data
- **DELETE** → Remove data

Each method represents a **clear intention**.

---

## ☕ Java Perspective (Very Important)

In Java backend applications:

- REST APIs are handled by **Controller classes**
- Each API maps to a controller method
- Controllers forward requests to services

Typical Java REST flow:

Client
↓
REST Controller
↓
Service Layer
↓
Repository
↓
Database

---

## 🔄 Request–Response Lifecycle

Step-by-step flow:

1. Client sends HTTP request
2. Controller receives and validates request
3. Service applies business logic
4. Repository interacts with database
5. Controller returns response

📌 This flow is consistent across most Java applications.

---

## 🎤 Interview One-Liners

- REST APIs use HTTP for communication
- Controllers handle incoming requests
- Services contain business logic
- Repositories manage data access

---

## ⚠️ Common Beginner Mistakes

- Writing logic in controllers
- Confusing REST APIs with frontend
- Ignoring HTTP method meanings
- Not understanding request flow
- Treating APIs as magic URLs

---

## ✅ Day 04 Summary

- REST APIs enable client–server communication
- Java controllers implement REST APIs
- Request flow follows clear layers
- Clean separation improves maintainability

---

## ⏭️ Next Day Preview

**Day 05 – Databases (SQL vs NoSQL Basics)**  
Understanding how data is stored and accessed in systems.
