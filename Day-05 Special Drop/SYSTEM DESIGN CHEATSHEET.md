# 🧠 SYSTEM DESIGN CHEATSHEET

### 🚀 Midway Boost — Day 05 Special Drop

<p align="center">
  <img src="https://img.shields.io/badge/System%20Design-Core-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Interview-Ready-success?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Beginner-Friendly-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Diagrams-ASCII%20%2B%20Visual-purple?style=for-the-badge"/>
</p>

<p align="center">
  <b>A single-file, high-signal revision sheet for System Design fundamentals.</b><br/>
  Built to impress recruiters, help interviews, and boost repo quality 🚀
</p>

---

## 📌 Coverage Scope (Till Day 05 Only)

✔ System Design Basics  
✔ Client–Server Architecture  
✔ Web Architecture  
✔ HTTP Request–Response Cycle  
✔ REST APIs  
✔ Monolithic Architecture  
✔ Microservices Architecture  
✔ Load Balancer  
✔ Databases (SQL vs NoSQL)  
✔ Caching

📎 **Visual Reference Folder:**  
`/assets/day05/`

---

## 1️⃣ What is System Design?

### 🧠 One-Line Definition

System Design is the process of **structuring software components** to meet **scalability, reliability, and performance** requirements.

### 🎯 Interview Line

> “System design focuses on how components interact under real-world load.”

## <img src="./Day-01/system-design-basics.png" alt="Basic System Design Diagram" width="650"/>

## 2️⃣ Client–Server Architecture

📷 Image:  
![Client Server Architecture](Day-02\client-server-architecture.jpg)
<img src="./Day-02\client-server-architecture">

### 🧠 One-Line Definition

Client sends requests, server processes them and sends responses.

### 🧩 ASCII Diagram

+---------+ Request +---------+
| Client | -------------------> | Server |
| (UI) | <------------------- | (Logic) |
+---------+ Response +---------+

### 🔁 Flow Summary

1. Client sends request
2. Server executes logic
3. Response returned

### 🎯 Interview Answer

> “Client handles presentation, server handles computation and data.”

---

## 3️⃣ Web Architecture (Browser → Server → Database)

📷 Image:  
![Web Architecture](./assets/day05/web-architecture.png)

### 🧠 One-Line Definition

Layered architecture separating **UI, business logic, and data**.

### 🧩 ASCII Diagram

+-----------+
| Browser |
+-----------+
|
v
+-----------+
| Web Server|
+-----------+
|
v
+-----------+
| Database |
+-----------+

### 🔁 Flow Summary

Browser → API → Logic → Database → Response

### 🎯 Interview Line

> “Layer separation improves maintainability and scalability.”

---

## 4️⃣ HTTP Request–Response Cycle

📷 Image:  
![HTTP Cycle](./assets/day05/http-cycle.png)

### 🧠 One-Line Definition

HTTP is a **stateless protocol** for client-server communication.

### 🧩 ASCII Diagram

Client Server
| ---- HTTP Req ---> |
| <--- HTTP Res ---- |

### 🔑 Key Points

- Stateless
- Uses status codes
- Supports multiple methods

### 🎯 Interview Tip

> “Server doesn’t remember previous requests.”

---

## 5️⃣ REST API Basics

📷 Image:  
![REST API](./assets/day05/rest-api.png)

### 🧠 One-Line Definition

REST is an architectural style using HTTP methods to manage resources.

### 🔧 Common Methods

GET → Read data
POST → Create data
PUT → Update data
DELETE → Remove data

### 🎯 Interview Line

> “REST APIs are stateless and resource-oriented.”

---

## ⚡ Ultra-Fast Interview Revision

- Client–Server → Request / Response
- HTTP → Stateless protocol
- REST → Resource-based APIs
- Load Balancer → Traffic distribution
- Cache → Speed optimization
- Monolith → Simplicity
- Microservices → Scalability

---

## 🏆 Why Recruiters ⭐ This File

✔ Clean structure  
✔ Diagram-based thinking  
✔ Interview language  
✔ Shows system intuition  
✔ Not tutorial-like — **professional**

---

## ⏭ Next Drop — Day 06

🔜 **Scalability Fundamentals**

- Vertical vs Horizontal Scaling
- Real-world system examples
- Advanced diagrams

> 💡 _If you understand this file, you already think like a system engineer._

---
