# Day 02 – Client–Server Architecture (Quick Notes)

---

## 🔹 What is Client–Server Architecture?

Client–Server Architecture is a software model where:

- A **client** sends a request
- A **server** processes that request
- The server sends a **response** back to the client

The client and server are **separate systems** with different responsibilities.

---

## 👤 Client – Key Points

A **client** is responsible for:

- Taking user input
- Sending requests to the server
- Displaying the response

Common examples:

- Web browsers (Chrome, Edge)
- Mobile applications
- Frontend frameworks (React, Angular)

📌 Clients do **NOT** handle business logic or database operations.

---

## 🖥️ Server – Key Points

A **server** is responsible for:

- Receiving client requests
- Executing business logic
- Communicating with databases
- Returning responses

📌 In this repository:
**Java Backend Application = Server**

Examples:

- Java Spring Boot app
- Java Servlet-based app

---

## 🔄 Request–Response Flow

Basic communication flow:

Client → Request → Server
Client ← Response ← Server

Key things to remember:

- Communication usually happens via **HTTP**
- Client waits for server response
- One server can handle many clients

---

## ☕ Java Perspective (Very Important)

In a Java backend system:

Client
↓
Java Controller
↓
Service Layer
↓
Repository
↓
Database

- Java backend acts as the **server**
- Database is accessed **only by the server**
- Client never talks to database directly

---

## 🎤 Interview One-Liners

- Client–Server architecture separates request and processing responsibilities
- Java backend applications typically act as servers
- Clients focus on UI, servers focus on logic and data

---

## ⚠️ Common Beginner Mistakes

- Treating frontend and backend as the same
- Putting business logic in client
- Thinking server serves only one client
- Ignoring request–response lifecycle
- Confusing database as part of client

---

## ✅ Day 02 Summary

- Client requests, server responds
- Java backend = server
- Clear separation of responsibilities
- Foundation of backend system design

---
