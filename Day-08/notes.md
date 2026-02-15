# 📝 Day 08 – Load Balancer Notes

## 🔹 Definition

A load balancer distributes incoming requests across multiple servers.

---

## 🔹 Why It Is Needed

Single server:

- Limited capacity
- Single point of failure

Multiple servers + load balancer:

- High availability
- Better performance
- Scalability

---

## 🔹 Basic Flow

Client → Load Balancer → One of many servers → Database

---

## 🔹 Key Benefit

Prevents server overload.

---

## 🔹 Traffic Distribution (Conceptual)

- Round Robin
- Least Connections
- IP Hash

Interview level: Just know names + purpose.

---

## 🔹 Java Developer’s Role

We do NOT build load balancer.

We:

- Build stateless applications
- Run multiple instances

Example:

Multiple Spring Boot instances behind a load balancer.

---

## 🔹 Stateless System

Any server can handle any request.

Used with:

- REST APIs
- JWT authentication

---

## 🔹 Stateful System Problem

Session stored in one server.

If request goes to another:
User loses session.

---

## 🔹 Interview One-Liner

Load balancer distributes traffic across multiple stateless servers for scalability and high availability.

---

## 🔹 Beginner Mistakes

- Thinking load balancer is code
- Over-explaining algorithms
- Ignoring stateless design

---

## 🔹 Real-World Examples

- NGINX
- AWS ELB
- HAProxy

(Concept only — no deep infra required)

---

## 🏁 After Day 08 You Can Explain

- Why multiple servers are needed
- Role of load balancer
- Stateless vs stateful
- How scalable systems handle traffic
