# 📝 Day 09 – URL Shortener (Beginner System Design) – Notes

---

## 🎯 One-Line Definition

A URL shortener converts a long URL into a short, unique URL and redirects users to the original link when accessed.

---

## 🧠 Why This System Is Important

This is your **first complete system design** where you learn:

- How to break a problem into components
- How services interact
- How database fits into design
- How scalability is introduced

It converts:

Theory → Real design thinking

---

## 🏗️ Functional Requirements

1. User submits a long URL
2. System returns a short URL
3. Short URL redirects to original URL

---

## ⚙️ Non-Functional Requirements (Beginner Level)

- Fast redirection
- High availability
- Scalable for large number of users

---

## 🧩 Core Components

### 1️⃣ Client

- Browser / Mobile App
- Sends HTTP request

---

### 2️⃣ Load Balancer

- Distributes traffic
- Improves availability
- Enables horizontal scaling

---

### 3️⃣ Application Service (Java – Spring Boot)

Responsible for:

- Generating short URL
- Saving mapping
- Redirecting users

---

### 4️⃣ Database

Stores mapping:

short_code → original_url

yaml
Copy code

---

## 🔄 Request Flow

### ➤ URL Shortening Flow

1. Client sends long URL
2. Request goes to Load Balancer
3. Load Balancer forwards to app instance
4. Service generates short code
5. Mapping stored in database
6. Short URL returned to user

---

### ➤ Redirection Flow

1. User hits short URL
2. Request goes to service
3. Service fetches original URL from DB
4. User is redirected

---

## ☕ Java Layer Mapping

### Controller

Handles:

POST /shorten
GET /{shortCode}

yaml
Copy code

---

### Service

Contains business logic:

- Generate short code
- Save mapping
- Fetch original URL

---

### Repository

- Talks to database

---

## 🔑 Short Code Generation (Beginner Safe)

We avoid complex hashing.

Simple approach:

1. Use auto-increment ID
2. Convert ID → Base62

Example:

ID: 100 → Base62 → "1C"

yaml
Copy code

Why Base62?

Because it uses:

a-z A-Z 0-9

yaml
Copy code

Which keeps URL short.

---

## 🗄️ Database Table Design

### url_mapping

| Field        | Purpose         |
| ------------ | --------------- |
| short_code   | Short URL key   |
| original_url | Actual long URL |

---

## ⚡ Performance Optimization (Concept Only)

### 1️⃣ Caching

Used because:

This is a **read-heavy system**

Frequently accessed URLs → Cache → Faster redirection

---

### 2️⃣ Stateless Application

Why?

So multiple instances can run behind load balancer.

---

## 📊 Read-Heavy Nature

Redirection happens more than URL creation.

So:

Read performance is critical.

---

## 🧠 Interview-Ready Explanation (30-Second Version)

User submits a long URL → load balancer routes the request → stateless Java service generates a short code → mapping stored in database → short URL returned.

When user accesses short URL → system fetches original URL → redirects.

---

## ❌ Common Beginner Mistakes

- Starting with microservices
- Over-scaling too early
- Using complex distributed ID generators
- Ignoring read-heavy nature
- Forgetting caching

---

## 🧠 Interview Power Lines

Use these lines:

- “This is a read-heavy system.”
- “We keep the service stateless for scalability.”
- “Caching improves redirection speed.”
- “Base62 encoding keeps URLs short and unique.”

---

## 🏁 What You Can Explain Now

After Day 09 you can:

✅ Design a complete system  
✅ Explain request flow  
✅ Identify components  
✅ Map system to Java layers  
✅ Talk in interview with confidence

---

## 🔥 Mental Model

Think in this order:

Requirements → Components → Flow → Database → Scalability

Not:

Code first ❌

---

## 📌 Revision Shortcut

URL Shortener =

Client → LB → Java Service → DB  
 ↘ Cache (for fast redirect)

---

## 🚀 Progress Upgrade

You are now capable of:

Explaining a real system design in a structured and interview-safe way.

This is a major milestone.
