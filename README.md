<h1 align="center">✨ Fullstack Chat & Video Calling App ✨</h1>

<p align="center">
  <img src="/frontend/public/image.png" alt="Demo App" width="800"/>
</p>

<p align="center">
  <b>💬 Real-time Chat • 📹 Video Calls • 🔐 Secure Auth • 🌍 Language Exchange Platform</b>
</p>

---

## 🌟 Overview

This is a **Fullstack Chat & Video Calling App** built using modern web technologies.  
It provides real-time **messaging, video calling, screen sharing**, and **recording features**, designed for a **language exchange community** or a **social platform**.

Users can chat, start video calls, react with emojis, and even record meetings — all in a beautiful, customizable UI with **32 unique themes**.

---

## 🧰 Tech Stack

| Area | Technologies Used |
|------|--------------------|
| **Frontend** | React, TailwindCSS, TanStack Query (React Query), Zustand |
| **Backend** | Node.js, Express.js, MongoDB, Mongoose |
| **Real-time & Video** | Stream SDK (Chat + Video), WebRTC |
| **Authentication** | JWT (JSON Web Tokens) |
| **Deployment** | Vercel (Frontend) & Render / Railway (Backend) |
| **Other Tools** | dotenv, bcryptjs, cors, axios |

---

## 🚀 Key Features

### 💬 Real-Time Chat
- Instant 1-on-1 and group messaging  
- Typing indicators & message reactions  
- Seen/unseen message status  
- Message history with timestamps  

### 📹 Video Calling
- 1-on-1 & group video calls  
- Screen sharing support  
- Video recording and playback  
- Mute/unmute audio & video  

### 🔐 Authentication & Authorization
- JWT-based login/signup  
- Protected routes & sessions  
- Secure password hashing using bcrypt  

### 🎨 Customization & UI
- 32 unique UI themes  
- Responsive design (desktop + mobile)  
- TailwindCSS for fast, modern styling  

### 🧠 State & Data Management
- Zustand for global state  
- TanStack Query for server caching and async data fetching  

### ⚙️ Error Handling
- Centralized backend error middleware  
- Toast notifications on frontend for user feedback  

---

## 📂 Folder Structure

```

📦 fullstack-chat-video-app
├── 📁 backend
│   ├── 📁 config          # Environment, DB, and Stream setup
│   ├── 📁 controllers     # Business logic for chat, auth, and calls
│   ├── 📁 models          # MongoDB models (User, Message, Conversation)
│   ├── 📁 routes          # API routes (auth, chat, call)
│   ├── 📁 middleware      # Auth + Error handling
│   └── server.js          # Main Express entry file
│
├── 📁 frontend
│   ├── 📁 src
│   │   ├── 📁 components  # UI components (chat box, video, etc.)
│   │   ├── 📁 pages       # Login, Signup, Chat, Call pages
│   │   ├── 📁 hooks       # Custom React hooks
│   │   ├── 📁 store       # Zustand state store
│   │   └── main.jsx       # React entry point
│   └── vite.config.js
│
└── README.md

````

---

## ⚙️ Environment Setup

### 🔧 Backend (`/backend`)

Create a `.env` file inside the `backend` folder:

```bash
PORT=5001
MONGO_URI=your_mongo_uri
STREAM_API_KEY=your_stream_api_key
STREAM_API_SECRET=your_stream_api_secret
JWT_SECRET_KEY=your_jwt_secret
NODE_ENV=development
````

### 💻 Frontend (`/frontend`)

Create a `.env` file inside the `frontend` folder:

```bash
VITE_STREAM_API_KEY=your_stream_api_key
```

---

## 🧪 Run the Project

### 🖥️ Start Backend Server

```bash
cd backend
npm install
npm run dev
```

Server runs on **[http://localhost:5001](http://localhost:5001)**

### 💻 Start Frontend

```bash
cd frontend
npm install
npm run dev
```

Frontend runs on **[http://localhost:5173](http://localhost:5173)**

---

## 🔍 API Endpoints Overview

| Method | Endpoint                | Description           |
| ------ | ----------------------- | --------------------- |
| `POST` | `/api/auth/register`    | Register new user     |
| `POST` | `/api/auth/login`       | Login existing user   |
| `GET`  | `/api/messages/:chatId` | Fetch chat messages   |
| `POST` | `/api/messages`         | Send a message        |
| `POST` | `/api/video/start`      | Initialize video call |
| `POST` | `/api/video/record`     | Start recording       |

---

## 🧠 Stream Integration

This app uses **Stream SDK** for:

* Real-time chat management
* Video conferencing (WebRTC)
* Screen sharing and recording

> 🧩 Get your keys from [https://getstream.io/](https://getstream.io/)

---

## 🌈 Screenshots

| Chat Interface                                         | Video Call                                   |
| ------------------------------------------------------ | -------------------------------------------- |
| ![Login UI](/frontend/public/login.png) | ![Video UI](/frontend/public/Video-call.png) |
| ![Chat UI](/frontend/public/Chat.png) | ![Video UI](/frontend/public/video-call.png) |

---

## 🌍 Deployment Guide

### Backend (Render / Railway)

1. Push your backend folder to GitHub
2. Deploy on [Render](https://render.com) or [Railway](https://railway.app)
3. Add all `.env` variables in dashboard

### Frontend (Vercel)

1. Push your frontend to GitHub
2. Import repo on [Vercel](https://vercel.com)
3. Add `VITE_STREAM_API_KEY` in environment variables

---

## 🧑‍💻 Contributing

Contributions are always welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazingFeature`)
3. Commit changes (`git commit -m 'Add new feature'`)
4. Push to branch (`git push origin feature/amazingFeature`)
5. Open a Pull Request 🎉

---

## 💬 Contact

📧 **Developer:** Vedant Agrawal
🌐 **GitHub:** (https://github.com/Vedant-Agrawal30)

---

## 📝 License

This project is licensed under the **MIT License** — free to use and modify with attribution.

---

<h3 align="center">⭐ If you like this project, don't forget to star it on GitHub! ⭐</h3>