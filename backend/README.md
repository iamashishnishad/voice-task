Backend (/backend)

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
