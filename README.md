# 🎬 YouTube Clone

A powerful full-stack YouTube Clone application that mirrors the core capabilities of a modern video-sharing platform. This project showcases scalable architecture, real-time interactions, and a polished user experience using current web development standards.

---

## 🚀 Features

### 🔐 User Authentication & Profile
- 🧾 Secure Registration – Multi-field signup with email validation, strong passwords, and duplicate prevention  
- 🔑 JWT Authentication – Token-based secure login with auto-refresh sessions  
- 👤 Profile Customization – Avatar upload, bio editing, and social links  
- 💾 Session Persistence – Auto login using secure localStorage  
- 🛡️ Account Security – Password hashing (bcrypt), protected routes, and safe logout  

---

### 🎥 Video Management & Streaming
- 📤 Upload System – Supports multiple formats with thumbnail generation and metadata extraction  
- ⚙️ Processing Pipeline – Background video optimization and adaptive streaming  
- 📝 Metadata Handling – Titles, descriptions, tags, categories, scheduling  
- 📊 Analytics – Track views, engagement, and performance  
- 🔒 Privacy Controls – Public, private, and unlisted videos  

---

### 💬 Social Interaction & Engagement
- 🧵 Comment System – Nested replies, mentions, and rich text support  
- 👍 Engagement Metrics – Real-time likes/dislikes with tracking  
- 📺 Subscriptions – Follow channels and manage notifications  
- 🕒 Watch History – Resume playback and track activity  
- 🔍 Content Discovery – Trending videos and personalized recommendations  

---

### 🎨 Professional UI/UX
- 📱 Responsive Design – Mobile-first, works on all devices  
- 🌙 Dark Mode – Clean YouTube-inspired theme  
- 🧩 Component-Based UI – Reusable React components  
- ✨ Interactive Elements – Animations, loaders, hover effects  
- ♿ Accessibility – ARIA labels, keyboard navigation, WCAG support  

---

## 🎯 Usage

### 🎬 For Creators
- Upload and organize videos efficiently  
- Build audience and manage subscribers  
- Access performance analytics  
- Ready for monetization features  

---

### 👀 For Viewers
- Discover videos via search and recommendations  
- Engage through comments and reactions  
- Sync watch history across devices  
- Share and interact socially  

---

### 💻 For Developers
- Learn scalable full-stack architecture  
- Follow industry best practices  
- Understand real-world tech integration  
- Easily extend and customize features  

---

## ⚙️ Setup Guide

### 📋 Prerequisites
- Node.js (v16+)  
- npm / yarn  
- MongoDB  

---

### 🖥️ Backend Setup

```bash
cd BackEnd
npm install
```

Create `.env` file:

```
PORT=8080
MONGO_URI=mongodb://127.0.0.1:27017/YOUTUBE
JWT_SECRET=dfsdjlarterthtretogojglkfjgldfg234565tr
```

Run server:

```bash
npm start
```

👉 Backend: http://localhost:8080  

---

### 🌐 FrontEnd Setup

```bash
cd FrontEnd
npm install
```

Add in `.env`:

```
VITE_BACKEND_SERVER=http://localhost:8080
```

Run FrontEnd:

```bash
npm run dev
```

👉 FrontEnd: http://localhost:5173  

---

## 🏗️ Project Architecture

### 🔙 Backend Structure
- ⚡ `server.js` → Entry point & server initialization  
- 🧠 `app.js` → Middleware & routing setup  

#### 📦 Database Layer
- `db.js` → MongoDB connection  
- `models/` → Schemas (User, Video, Channel, Comment)  

#### 🎯 Controllers
- Handle business logic (auth, video, channel, comment, actions)  

#### 🛣️ Routes
- Define API endpoints  

#### 🧩 Middleware
- Auth validation  
- Input validation  
- Error handling  

---

### 🎨 Frontend Structure

#### Core
- `main.jsx` → App bootstrap  
- `App.jsx` → Routing & layout  

#### Pages
- Login, Register, Homepage, Video player  

#### Components
- Header, VideoCard, CommentSection, Toast, Forms  

#### State Management
- Context API  
- Redux Toolkit  

#### Services
- Axios API layer  

---

## 🛠️ Tech Stack

### 🔙 Backend
- Node.js  
- Express.js  
- MongoDB + Mongoose  
- JWT  
- bcrypt  
- dotenv  

---

### 🎨 Frontend
- React  
- Vite  
- Tailwind CSS  
- Redux Toolkit  
- React Router  
- Axios 
- dotenv 

---

## 🔗 API Overview

### 🔐 Authentication
```
POST /api/auth/register
POST /api/auth/login
```

### 🎥 Videos
```
POST /api/videos
GET /api/videos
```

### 👍 Engagement
```
POST /api/actions/likes
```

### 💬 Comments
```
GET /api/comments/:videoId
POST /api/comments
```

---

## ✅ Best Practices
- 🧱 Modular architecture  
- 🔄 Separation of concerns  
- 🔐 Strong security implementation  
- ⚡ Performance optimization (caching, lazy loading)  
- 📈 Scalable and maintainable code  

---

## 🧪 Testing Strategy
- Unit Testing  
- Integration Testing  
- End-to-End Testing  
- Performance Testing  
- Security Testing  

---

## 📌 Repository

👉 GitHub: https://github.com/gautam-vaishnav016/YOUTUBE_CLONE