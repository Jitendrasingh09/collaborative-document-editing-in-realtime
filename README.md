# 📄 Real-Time Collaborative Document Editor

## 🚀 Introduction
In today's interconnected world, seamless collaboration on documents among multiple users is essential for productivity and efficiency. **The Real-Time Collaborative Document Editor** is a cutting-edge application designed to enable **multiple users to edit shared documents simultaneously in real time**.

This project leverages **modern web technologies** like **NestJS** for backend services, **WebSockets** for real-time communication, and robust **authentication & authorization mechanisms** to ensure **data security and user privacy**.

---

## ✨ Key Features
- **Real-Time Collaboration** – Multiple users can edit the same document instantly.  
- **Document & User Management** – Efficiently manage documents and track users.  
- **WebSocket–Database Mapping** – Identify and map WebSocket clients to authenticated database users.  
- **Authentication & Authorization** – Secure login and role-based access control using JWT.  
- **Conflict Resolution** – Prevent and manage conflicting edits.  
- **Persistence** – Auto-save and store document changes in a database.  
- **DTO Management** – Maintain clean data flow using **Data Transfer Objects**.  
- **Validation & Transformation** – Utilize **class-validator** and **class-transformer** for data integrity.

---

## 🛠️ Technology Stack

**Frontend**
- ReactJS  
- Context API (state management)  
- TailwindCSS

**Backend**
- NestJS  
- WebSocket Gateway & Socket.io-client  
- Mongoose & MongoDB Atlas  
- JWT (HMAC with SHA-256)  
- TypeScript

---


## 📂 Project Structure

```text
collaborative-document-editing-in-realtime/
│
├── src/
│   ├── app.module.ts                  # Main application module
│   ├── document/                      # Document module
│   │   ├── document.controller.ts     # Handles document-related HTTP requests
│   │   ├── document.service.ts        # Business logic for documents
│   │   ├── document.entity.ts         # Mongoose schema for documents
│   │   └── document.module.ts         # Document module definition
│   │
│   ├── auth/                          # Authentication module
│   │   ├── auth.controller.ts         # Handles login & registration
│   │   ├── auth.service.ts            # JWT-based authentication logic
│   │   ├── jwt.strategy.ts            # JWT strategy configuration
│   │   ├── guards/                    # Authentication guards
│   │   │   └── jwt-guards.auth.ts     # JWT guard for protecting routes
│   │   └── auth.module.ts             # Auth module definition
│   │
│   ├── user/                          # User module
│   │   ├── user.controller.ts         # Handles user-related requests
│   │   ├── user.service.ts            # Business logic for users
│   │   ├── user.entity.ts             # Mongoose schema for users
│   │   └── user.module.ts             # User module definition
│   │
│   ├── socket.gateway.ts              # WebSocket event handling
│   └── main.ts                        # Application entry point
│
├── .env                               # Environment variables
└── package.json                       # Dependencies & scripts
```
---

## 🎥 Video Demo

**Frontend**
- Part 1 – https://www.loom.com/share/ef97f7ba1e16435baf3506f7e2333ab8?sid=9ab4cb8c-39a9-48ea-9cde-c55c023b6e76  
- Part 2 – https://www.loom.com/share/db0d9a09a1a64a1196e2fb717db1fea2?sid=82fe327b-9ff7-4d4b-88e8-871ac0c95c7b

**Backend**
- Demo – https://www.loom.com/share/d32ac1f69e454fbab57841eb05fe958a?sid=1b64a82b-9707-4481-908b-3f087d283069

---

## 📸 Project Snapshots

![Screenshot 19](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/4e9c93d3-9b8d-4170-8683-41b3c9cdf44d)  
![Screenshot 21](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/d8d46bcc-af22-40d3-964e-707766b51522)  
![Screenshot 22](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/37f102ba-e5d4-4083-8b7f-660db28e2cb9)  
![Screenshot 26](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/bec637a6-c544-4f26-877b-5cd6dc594647)  
![Screenshot 28](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/ee8a2558-3320-40be-9f96-b40d3f5e2c16)  
![Screenshot 33](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/b7bea3c8-584d-4247-924f-dbe96bc2bd24)  
![Screenshot 35](https://github.com/tikhepooja11/Realtime-collaborative-document-editing-app/assets/47672660/179da481-b196-410e-a4ce-d56cd1b43442)

---

## 📌 How It Works
1. **User Authentication** – Users log in or register using JWT-based authentication.  
2. **Document Access** – Authenticated users can create, edit, and view documents.  
3. **Real-Time Sync** – WebSockets ensure that changes are instantly reflected for all connected users.  
4. **Data Persistence** – Changes are saved in MongoDB Atlas for future access.  
5. **Conflict Resolution** – Handles multiple simultaneous edits without data loss.

---

## 📜 License
This project is licensed under the **MIT License**. You are free to use, modify, and distribute it.

