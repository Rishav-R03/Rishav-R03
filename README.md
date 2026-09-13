<h1 align="center">Hi 👋, I'm Rishav Raj</h1>

<h3 align="center">
Backend Engineer • Go Developer • Distributed Systems Enthusiast
</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
</p>

---

## About Me

I'm a backend engineer focused on building reliable, scalable, and performance-oriented systems using Go.

My interests lie at the intersection of:

* Distributed Systems
* Concurrent Programming
* Backend Architecture
* Database Internals
* Messaging Systems
* Performance Engineering

I enjoy understanding not only how systems work, but why specific design decisions are made and what tradeoffs exist behind them.

Currently diving deeper into:

* PostgreSQL Internals (MVCC, WAL, Transactions)
* Redis & Caching Patterns
* Messaging Systems (RabbitMQ & Kafka)
* Distributed System Design
* Go Runtime & GMP Scheduler

---

## 🚀 Featured Projects
### 🚀 Distributed Rate Limiter & Request Throttler
Checkout -> https://github.com/Rishav-R03/distributed-rate-limiter

Production-inspired distributed rate limiting service built in Go using Redis, Lua scripting, PostgreSQL, Prometheus, and Docker.

**Tech Stack:** Go • Redis • Lua • PostgreSQL • Prometheus • Grafana • Docker

**Highlights**

* Engineered a distributed sliding-window rate limiter capable of handling high request throughput while maintaining sub-millisecond decision latency.
* Implemented atomic Redis Lua scripts to eliminate race conditions and ensure correctness under concurrent traffic.
* Built an asynchronous analytics pipeline using worker pools and PostgreSQL to decouple request processing from metrics persistence.
* Designed failure-aware middleware capable of graceful degradation during Redis outages to preserve service availability.
* Integrated observability using Prometheus and Grafana for latency, throughput, and rate-limit analytics.
* Load-tested the system under sustained traffic using k6 and Vegeta.

---

### 📊 Event-Driven CQRS Analytics Engine
Checkout -> https://github.com/Rishav-R03/food_delivery_Analytics_Platform

A production-inspired analytics platform demonstrating how modern food-delivery systems process transactional workloads and serve analytical insights in near real time.

**Tech Stack:** Go • PostgreSQL • CDC • Docker • Prometheus • k6

**Highlights**

* Architected a CQRS-based microservices system separating transactional OLTP workloads from analytical OLAP workloads.
* Built an event-driven CDC pipeline using PostgreSQL LISTEN/NOTIFY to synchronize operational and analytical databases.
* Designed denormalized fact-table analytics models optimized for dashboard-style queries and reporting workloads.
* Developed independent Order Service, CDC Worker, and Analytics Service components communicating through asynchronous event flows.
* Implemented observability, structured logging, and performance benchmarking to validate system reliability under load.
* Demonstrated real-world backend patterns used in large-scale data-intensive applications.

---

### ☕ JVMAnalyze — JVM Profiling & Performance Diagnostics Tool
Checkout -> https://github.com/Rishav-R03/JVMAnalyze

A JVM observability and diagnostics platform for monitoring application performance, analyzing garbage collection behavior, and detecting memory leaks.

**Tech Stack:** Java • JMX • JVM Internals • Maven • Log4j

**Highlights**

* Built a real-time JVM monitoring platform collecting heap, thread, garbage collection, and runtime telemetry through JMX instrumentation.
* Developed a GC analytics engine capable of parsing and analyzing high-frequency garbage collection events across multiple GC algorithms.
* Implemented automated memory-leak detection using trend-analysis techniques to identify abnormal heap growth patterns before failures occur.
* Generated actionable performance reports containing latency distributions, GC efficiency metrics, and tuning recommendations.
* Designed a terminal-based monitoring dashboard providing low-latency visibility into JVM health and resource utilization.
* Enabled comparative analysis of JVM behavior across different garbage collectors and runtime configurations.

---

## 🛠 Tech Stack

### Languages

* Go
* Java
* SQL

### Backend Development

* REST APIs
* Microservices
* Concurrent Programming
* Event-Driven Architecture
* Worker Pools
* API Design

### Databases

* PostgreSQL
* Redis

### Messaging & Infrastructure

* RabbitMQ
* Docker

### Monitoring & Observability

* Prometheus
* Grafana

### Core Concepts

* Concurrency
* Caching
* Transactions
* Database Design
* Message Queues
* Distributed Systems Fundamentals

---

## 📚 Currently Learning

* Advanced Data Structures & Algorithms
* PostgreSQL Internals
* Redis Internals
* Kafka
* Distributed Systems
* Go Runtime Internals
* System Design

---

## 🎯 2027 Goals

* Build production-grade distributed systems
* Contribute to open-source Go projects
* Deepen expertise in databases and messaging systems
* Publish technical write-ups on backend engineering
* Land a high-impact Backend / Platform Engineering role

---

## 📫 Connect With Me

* Email: **[rishav042023@gmail.com](mailto:rishav042023@gmail.com)**
* LinkedIn: [**[LinkedIn]**](https://www.linkedin.com/in/rishav-raj-15b077249/)
* GitHub: **[GitHub](https://github.com/Rishav-R03)**

---

<p align="center">
  <i>"First make it work. Then make it correct. Then make it fast."</i>
</p>
