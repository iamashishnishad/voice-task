# 🎤 Voice-Enabled Task Tracker

A full-stack productivity application that allows you to create tasks by speaking naturally. The system intelligently parses voice input to extract task details like title, priority, due date, and status.

**Live Demo:** [Frontend](https://voice-task-frontend-17op.onrender.com) | [Backend API](https://voice-task-backend-xd9b.onrender.com)

## ✨ Features

### 🎤 Voice Input (AI-Powered)
- **Natural Language Processing**: Speak tasks like you're talking to a colleague
- **Smart Parsing**: Extracts title, priority, due date, and status from speech
- **Speech Recognition**: Built-in browser speech-to-text
- **Auto-Correction**: Fixes common speech recognition errors (e.g., "gh period" → "high priority")
- **Auto-Create**: Add "create this" at the end to automatically save tasks

### 📋 Task Management
- **Kanban Board**: Drag-and-drop tasks between To Do, In Progress, and Done
- **List View**: Table view with filtering and sorting
- **Full CRUD**: Create, Read, Update, Delete tasks
- **Search & Filter**: Filter by status, priority, or search by text
- **Responsive Design**: Works on desktop and mobile

### 🛠 Technical Features
- **Real-time Updates**: Immediate UI feedback
- **Error Handling**: Graceful error states and user notifications
- **Health Monitoring**: API status monitoring
- **CORS Configured**: Proper cross-origin support for deployment

---

## 🏗 AI Tool
ChatGpt
DeepSeek



---

## 🚀 Quick Start

### Prerequisites
- Node.js 16+ 
- npm or yarn
- MongoDB (Local or Atlas)
- Modern browser with microphone access

### Option 1: One-Command Setup (Recommended)
```bash
# Clone the repository
git clone https://github.com/yourusername/voice-task-tracker.git
cd voice-task-tracker

# Run setup script
chmod +x setup.sh
./setup.sh


Backend Setup
# Navigate to backend
cd backend

# Install dependencies
npm install

# Configure environment
cp .env.example .env
# Edit .env with your MongoDB URI

# Seed database with sample tasks
npm run seed

# Start development server
npm run dev
# Server runs on http://localhost:5001


backend/
├── models/
│   └── Task.js              # MongoDB task schema
├── routes/
│   ├── tasks.js             # Task CRUD operations
│   └── voice.js             # Voice parsing logic
├── middleware/
│   └── errorHandler.js      # Centralized error handling
├── .env.example             # Environment variables template
├── server.js               # Express server setup
├── seed.js                 # Database seeding
└── package.json            # Dependencies and scripts


Frontend

# Navigate to frontend
cd frontend

# Install dependencies
npm install

# Start development server
npm start
# App runs on http://localhost:3000

frontend/
├── src/
│   ├── components/
│   │   ├── Layout.js        # Main layout with navigation
│   │   ├── VoiceRecorder.js # Voice input component
│   │   ├── TaskForm.js      # Task creation/editing form
│   │   ├── TaskItem.js      # Individual task display
│   │   ├── Column.js        # Kanban column
│   │   └── ErrorBoundary.js # React error boundary
│   ├── features/
│   │   └── tasks/
│   │       └── tasksSlice.js # Redux slice for tasks
│   ├── pages/
│   │   ├── Dashboard.js     # Kanban board view
│   │   └── TaskList.js      # List view
│   ├── app/
│   │   └── store.js         # Redux store configuration
│   ├── App.js              # Root component
│   └── index.js            # Application entry point
├── public/
│   └── index.html          # HTML template
└── package.json            # Dependencies and scripts
