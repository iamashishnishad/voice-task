Frontend Setup
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