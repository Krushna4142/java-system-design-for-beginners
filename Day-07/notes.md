# 📝 Day 07 – Caching (Why & Where)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## 📌 1️⃣ What is Caching?

Caching is the process of storing frequently accessed data in a temporary storage area (called cache) to improve performance and reduce load on the main system.

👉 Instead of fetching data again and again from:

- Database
- External API
- Disk

We store it in:

- Memory
- Fast storage layer

So next time → Response is faster ⚡

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## 📌 2️⃣ Why Do We Need Caching?

### 🚀 1. Improve Performance

Database queries are slow compared to memory.
Cache reduces response time.

### 📉 2. Reduce Database Load

Less repeated queries = less DB pressure.

### 💰 3. Reduce Cost

Less API calls = lower cloud cost.

### 📈 4. Increase Scalability

Handles more users without increasing servers.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## 📌 3️⃣ Where is Caching Used?

### 🔹 1. Browser Cache

Stores:

- Images
- CSS
- JS files

Example:
When you revisit a website → It loads faster.

### 🔹 2. Application-Level Cache

Inside backend server memory.

Example:

- Storing product details
- Storing user session data

### 🔹 3. Database Query Cache

Database stores recent query results.

### 🔹 4. Distributed Cache

Used in scalable systems.

Popular tools:

- Redis
- Memcached

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## 📌 4️⃣ Types of Caching

### 1️⃣ Client-Side Cache

Stored in browser.

### 2️⃣ Server-Side Cache

Stored in backend server memory.

### 3️⃣ CDN Cache

Stored in distributed servers worldwide.

Example:
Cloudflare CDN

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## 📌 5️⃣ Cache Workflow

Step 1: Client requests data  
Step 2: Server checks cache  
Step 3:  
 • If present → Return from cache (Cache Hit)  
 • If not present → Fetch from DB (Cache Miss)  
Step 4: Store result in cache  
Step 5: Return response

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## 📌 6️⃣ Important Terms

### 🔹 Cache Hit

Data found in cache.

### 🔹 Cache Miss

Data not found → fetched from DB.

### 🔹 TTL (Time To Live)

How long data stays in cache.

Example:
TTL = 10 minutes → After 10 minutes data expires.

### 🔹 Cache Eviction

Removing old data from cache.

Policies:

- LRU (Least Recently Used)
- FIFO (First In First Out)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## 📌 7️⃣ Real World Example

Without Cache:
User → Server → Database → Server → User  
(Time = Slow)

With Cache:
User → Server → Cache → Server → User  
(Time = Fast ⚡)

Example:
E-commerce site product page.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## 📌 8️⃣ When NOT to Use Cache?

❌ Frequently changing data  
❌ Sensitive real-time data  
❌ Small systems with low traffic

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## 🎯 Interview Questions

1. What is caching?
2. What is cache hit and miss?
3. What is TTL?
4. Explain LRU policy.
5. Difference between client-side and server-side caching?

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## 🏆 Summary

✔ Caching improves performance  
✔ Reduces database load  
✔ Increases scalability  
✔ Works best for frequently accessed data  
✔ Use TTL and eviction policies carefully

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

```

```
