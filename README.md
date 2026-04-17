# Softy Pinko Docker Project

## 📌 Overview

This project demonstrates how to build, containerize, and deploy a full-stack web application using Docker and Docker Compose.

The application consists of:

* A **Front-end** (served with Nginx)
* A **Back-end API** (Flask)
* A **Reverse Proxy** (Nginx)
* **Load balancing** across multiple API servers

---

## 🧱 Project Structure

```
holbertonschool-softy-pinko-docker/
├── task0/   # Basic Docker image
├── task1/   # Flask API container
├── task2/   # Front-end with Nginx
├── task3/   # Front-end + Back-end integration
├── task4/   # Docker Compose setup
├── task5/   # Reverse proxy with Nginx
├── task6/   # Horizontal scaling (multiple API servers)
```

---

## 🐳 Technologies Used

* Docker
* Docker Compose
* Nginx
* Python (Flask)
* JavaScript (AJAX / jQuery)

---

## 🚀 How to Run (Task 5 - Full App)

Navigate to task5:

```
cd task5
```

Build and run:

```
docker-compose build
docker-compose up
```

Open in browser:

```
http://localhost
```

---

## 🔄 API Endpoint

```
GET /api/hello
```

Response:

```
Hello, World!
```

---

## 🌐 Architecture

Client (Browser)
↓
Nginx Proxy (Port 80)
↓
├── Front-end (Port 9000)
└── Back-end API (Port 5252)

---

## ⚖️ Load Balancing (Task 6)

To scale the API servers:

```
docker-compose up --scale back-end=2
```

This will:

* Run multiple backend containers
* Distribute requests using **round-robin**

---

## 🎯 Key Features

* Containerized full-stack application
* Reverse proxy routing
* API integration using AJAX
* Docker Compose orchestration
* Horizontal scaling with load balancing

---



## 👩‍💻 Author

* Rateel Bahathek
