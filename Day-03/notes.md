# Day 03 – Monolith vs Layered Architecture (Quick Notes)

---

## 🔹 What is a Monolithic Application?

A **monolithic application** is:

- Built as a **single unit**
- Deployed as **one application**
- All features live in one codebase

📌 Most Java backend applications start as monoliths.

---

## 🧱 What is Layered Architecture?

Layered architecture organizes a monolithic application into **logical layers**.

Each layer has a **single responsibility**.

Typical Java layers:

- Controller Layer
- Service Layer
- Repository Layer
- Database

---

## ☕ Java Perspective (Very Important)

Most real-world Java apps are:

> **Layered Monolithic Applications**

Meaning:

- One deployable Java application
- Internally structured using layers

Common package structure:

controller/
service/
repository/
model/

This structure:

- Improves readability
- Makes testing easier
- Reduces tight coupling

---

## 🔄 Request Flow in Layered Architecture

Client
↓
Controller
↓
Service
↓
Repository
↓
Database

Rules:

- Controller → handles HTTP only
- Service → business logic only
- Repository → database access only

---

## 🎤 Interview One-Liners

- A monolith is deployed as a single unit
- Layered architecture separates responsibilities
- Most Java apps use layered monolithic design
- Monoliths are not bad by default

---

## ⚠️ Common Beginner Mistakes

- Assuming monolith means poor design
- Skipping service layer
- Writing SQL in controller
- Jumping to microservices too early
- Overcomplicating simple applications

---

## ✅ Day 03 Summary

- Monolith = single application
- Layers = internal structure
- Java apps commonly follow layered architecture
- Clean layering improves maintainability

---

## ⏭️ Next Day Preview

**Day 04 – REST APIs & Request Flow**  
Understanding how HTTP requests move through Java layers.
