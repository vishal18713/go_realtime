# 🚀 Inox - Real-Time Collaboration Platform

> A scalable real-time communication platform built with **Go**, **React**, **WebSockets**, **WebRTC**, **PostgreSQL**, and **Redis**, designed for low-latency messaging, media streaming, and collaborative applications.

---

## 📌 Overview

**Inox** is a production-oriented full-stack real-time communication system that enables users to communicate instantly through persistent WebSocket connections while supporting media streaming using WebRTC.

The project follows a modular backend architecture written in **Go**, a modern **React + TypeScript** frontend, and a dedicated **Admin Portal** for monitoring system health and application metrics.

The system is designed with scalability, maintainability, and performance in mind.

---

# ✨ Features

### 👤 Authentication

* User Signup
* User Login
* Secure Logout
* Session management
* Protected APIs

---

### ⚡ Real-Time Communication

* Persistent WebSocket connections
* Low-latency messaging
* Real-time event broadcasting
* Multi-user room support
* Presence updates

---

### 🎥 Media Streaming

* WebRTC integration
* Peer-to-peer communication
* Audio/Video support
* Low-latency media transport

---

### 💬 Chat System

* Instant messaging
* Room-based communication
* Real-time message delivery
* Scalable event handling

---

### 🏠 Room Management

* Create Rooms
* Join Rooms
* Leave Rooms
* Room lifecycle management
* Concurrent participants

---

### 📊 Admin Dashboard

* Live application telemetry
* System monitoring
* Metrics visualization
* WebSocket-based live updates
* Health monitoring

---

### 📈 Observability

* Health Check endpoint
* Metrics endpoint
* Logging
* Runtime telemetry
* Monitoring APIs

---

### ⚙️ Infrastructure

* PostgreSQL integration
* Redis caching
* Docker support
* Environment-based configuration
* Modular services

---

# 🏗️ Project Architecture

```
                     +-------------------+
                     |   React Frontend  |
                     +---------+---------+
                               |
                               |
                         HTTP / WebSocket
                               |
                +--------------+--------------+
                |      Go Backend Server      |
                +--------------+--------------+
                       |                |
                  PostgreSQL         Redis
                       |
                  Persistent Data

                WebRTC Peer Connections
                       |
                  Media Streaming
```

---

# 🛠️ Tech Stack

## Backend

* Go (Golang)
* WebSockets
* WebRTC (Pion)
* PostgreSQL
* Redis
* JWT Authentication
* REST APIs

---

## Frontend

* React
* TypeScript
* Vite
* React Router

---

## Admin Portal

* React
* TypeScript
* Live Monitoring Dashboard

---

## Infrastructure

* Docker
* Docker Compose
* Environment Variables

---

# 📂 Project Structure

```
inox/

├── backend/
│   ├── cmd/
│   ├── internal/
│   ├── migrations/
│   └── pkg/
│
├── frontend/
│   ├── src/
│   └── public/
│
├── admin-portal/
│   ├── src/
│   └── public/
│
├── docker-compose.yml
├── Makefile
└── README.md
```

---

# 🚀 Getting Started

## Clone Repository

```bash
git clone https://github.com/yourusername/inox.git

cd inox
```

---

## Backend

```bash
cd backend

go mod download

go run cmd/server/main.go
```

---

## Frontend

```bash
cd frontend

npm install

npm run dev
```

---

## Admin Portal

```bash
cd admin-portal

npm install

npm run dev
```

---

# 🐳 Docker

Run the complete application using Docker Compose.

```bash
docker-compose up --build
```

---

# 🔧 Environment Variables

Create a `.env` file inside each service.

Example:

```env
DATABASE_URL=

REDIS_URL=

JWT_SECRET=

PORT=
```

Refer to the included `.env.example` files for the complete configuration.

---

# 📡 API Endpoints

### Authentication

```
POST /api/v1/auth/signup

POST /api/v1/auth/login

POST /api/v1/auth/logout
```

---

### Health

```
GET /healthz
```

---

### Metrics

```
GET /metrics
```

---

### Admin

```
GET /api/v1/admin/telemetry

GET /api/v1/admin/telemetry/ws
```

---

# ⚡ Performance Highlights

* Persistent WebSocket connections
* Low-latency real-time communication
* Redis-powered caching
* Efficient concurrent processing using Go routines
* Scalable modular architecture
* Production-ready REST APIs

---

# 🎯 Design Principles

* Clean Architecture
* Modular Codebase
* Separation of Concerns
* Scalable Services
* Dependency Injection
* Environment-based Configuration

---

# 📈 Future Improvements

* Horizontal scaling
* Kubernetes deployment
* Distributed WebSocket gateway
* Message persistence
* Push notifications
* File sharing
* Screen sharing
* Recording support
* End-to-end encryption
* OAuth authentication

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push your branch
5. Open a Pull Request

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

Developed as a production-oriented real-time communication platform showcasing scalable backend architecture, concurrent programming in Go, and modern React-based frontend development.
