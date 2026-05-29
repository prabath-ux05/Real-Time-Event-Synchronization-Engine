# TweetX - Real-Time Event Synchronization Engine

![Java](https://img.shields.io/badge/Java-17-orange)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-green)
![WebSocket](https://img.shields.io/badge/WebSocket-Real--Time-blue)
![JPA](https://img.shields.io/badge/Spring%20Data%20JPA-Persistence-success)
![H2](https://img.shields.io/badge/H2-Database-lightgrey)
![Maven](https://img.shields.io/badge/Maven-Build-red)

---

## 📌 Overview

The Real-Time Event Synchronization Engine is a WebSocket-powered communication platform designed to synchronize user events, messaging activities, and conversation state across connected clients in real time.

Built using Spring Boot, WebSockets, and JPA, the system enables low-latency communication, online user tracking, persistent messaging, and session-aware interactions without relying on repetitive client polling.

The project demonstrates practical implementation of event-driven architectures, real-time synchronization mechanisms, WebSocket communication workflows, and backend system design principles commonly used in modern collaborative applications.

---

## 🎥 Demo Video

<p align="center">
  <a href="https://drive.google.com/file/d/1ULnT7dYohjQ_oIHFZywwxaxyP5liCw5K/view?usp=drive_link">
    <img src="docs/Signup Page.png" width="900">
  </a>
</p>

<p align="center">
  <strong>Click the preview image to watch the complete TweetX demonstration.</strong>
</p>

---
## ✨ Core Features

### 💬 Real-Time Messaging

- Instant message delivery
- Bidirectional communication
- Persistent conversation history
- Session-aware messaging

### 👤 User Authentication

- User Registration
- Secure Login Flow
- Session Management
- User Validation

### 🟢 Presence Synchronization

- Online User Detection
- Live Status Updates
- Connection Tracking
- Session Monitoring

### 📂 File Sharing

- File Upload Support
- Shared Resources
- Upload Persistence

### ⚡ Event Synchronization

- Real-Time Event Broadcasting
- WebSocket-Based Updates
- Reduced Polling Overhead
- Low-Latency Communication

---

## 🏗️ System Architecture

```text
┌───────────────┐
│ Browser Client│
└───────┬───────┘
        │
        ▼

┌─────────────────────┐
│ Spring Boot Backend │
└─────────┬───────────┘
          │
          ▼

 ┌──────────────┐
 │ Authentication│
 └──────────────┘

 ┌──────────────┐
 │ WebSocket Hub│
 └──────────────┘

 ┌──────────────┐
 │ Message Store│
 └──────────────┘

 ┌──────────────┐
 │ H2 Database  │
 └──────────────┘
```

---

<details>
<summary><strong>⚙️ Tech Stack</strong></summary>

### ☕ Backend

- Java 17
- Spring Boot 3
- Spring MVC
- Spring WebSocket
- Spring Data JPA

### 🗄️ Database

- H2 Database
- Hibernate ORM

### 🌐 Communication

- WebSocket Protocol
- Session-Based Communication

### 🎨 Frontend

- HTML
- CSS
- JavaScript

### 📦 Build Tools

- Maven

</details>

---

## 🔄 Event Synchronization Workflow

```text
User Action → WebSocket Event → Server Processing → Event Broadcast → Connected Clients
```

---

## 💬 Messaging Workflow

```text
Sender → WebSocket Channel → Message Validation → Database Persistence → Receiver
```

---

## 🖼️ Platform Preview

### 🔐 User Authentication

<p align="center">
  <img src="docs/Signup Page.png" width="80%">
</p>

### 💬 Real-Time Messaging

<p align="center">
  <img src="docs/Chat Page.png" width="80%">
</p>

---

<details>
<summary><strong>📁 Project Structure</strong></summary>

```text
Real-Time-Event-Synchronization-Engine/
│
├── src/main/java/
│   ├── controller/
│   │   ├── AuthController.java
│   │   ├── MessageController.java
│   │   └── FileUploadController.java
│   │
│   ├── model/
│   │   ├── User.java
│   │   └── Message.java
│   │
│   ├── repository/
│   │   ├── UserRepository.java
│   │   └── MessageRepository.java
│   │
│   ├── config/
│   │   └── WebMvcConfig.java
│   │
│   ├── MyWebSocketHandler.java
│   ├── WebSocketConfig.java
│   └── DemoApplication.java
│
├── src/main/resources/
│   ├── static/
│   ├── application.properties
│
├── docs/
│   ├── Signup Page.png
│   └── Chat Page.png
│
├── uploads/
├── pom.xml
└── README.md
```

</details>

---

## 🔌 API Architecture

```text
Client
  │
  ▼
REST Controllers
  │
  ▼
Service Layer
  │
  ▼
Repositories
  │
  ▼
H2 Database
```

---

## ☁️ Real-Time Communication Layer

The platform uses WebSocket technology to establish persistent bidirectional communication channels between clients and the server.

### Benefits

- Instant event propagation
- Reduced network overhead
- Lower latency communication
- Efficient state synchronization
- Improved user experience

---

## 📊 Event Processing Pipeline

```text
Client Request → Authentication → WebSocket Processing → Message Persistence → Event Broadcast → Client Synchronization
```

---

## 🗄️ Database Layer

The application utilizes H2 Database with Spring Data JPA for persistence and entity management.

### Stored Data

- User Accounts
- Conversation History
- Uploaded Files
- Session Information

### Benefits

- Lightweight Development Database
- Easy Configuration
- Fast Local Development
- JPA Repository Integration

---

## 🚀 Local Development Setup

### Clone Repository

```bash
git clone https://github.com/yourusername/Real-Time-Event-Synchronization-Engine.git

cd Real-Time-Event-Synchronization-Engine
```

### Build Project

```bash
mvn clean install
```

### Run Application

```bash
mvn spring-boot:run
```

### Access Application

```text
http://localhost:8080
```

---

## 🔐 Configuration

### application.properties

```properties
spring.datasource.url=jdbc:h2:file:./data/chatdb
spring.datasource.driverClassName=org.h2.Driver

spring.jpa.hibernate.ddl-auto=update

spring.h2.console.enabled=true
```

---

## 🛠️ Engineering Highlights

- WebSocket-Based Real-Time Communication
- Event-Driven Architecture
- Session-Based Authentication
- Persistent Message Storage
- Online User Synchronization
- File Upload Integration
- Spring MVC Architecture
- Spring Data JPA Integration
- Repository Design Pattern
- H2 Embedded Database
- Low-Latency Event Broadcasting

---

## 🎯 Learning Outcomes

This project demonstrates practical experience with:

- Real-Time System Design
- Event-Driven Architectures
- WebSocket Communication
- Spring Boot Development
- Backend API Design
- Database Persistence
- Session Management
- Full-Stack Application Development

---

## 🔮 Future Enhancements

### Communication

- Group Chat Support
- Message Reactions
- Read Receipts
- Typing Indicators

### Security

- Spring Security Integration
- JWT Authentication
- Password Encryption
- Role-Based Access Control

### Scalability

- PostgreSQL Migration
- Redis Pub/Sub
- Kafka Event Streaming
- Horizontal Scaling

### Observability

- Prometheus Monitoring
- Grafana Dashboards
- Centralized Logging
- Distributed Tracing

---

## 📄 License

This project is intended for educational, learning, and portfolio demonstration purposes.

---

## 👨‍💻 Author

**Prabath D**
