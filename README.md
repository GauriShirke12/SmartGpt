# SmartGpt

A full-stack ChatGPT-like application built with React and Node.js, featuring a clean chat interface with conversation threading and persistent storage.

## 🚀 Features

- **Interactive Chat Interface**: Clean and responsive UI for chatting with OpenAI's GPT models
- **Conversation Threading**: Organize chats into separate threads for better context management
- **Chat History**: View and access previous conversations
- **Real-time Responses**: Stream responses from OpenAI API
- **Persistent Storage**: Save chat history using MongoDB
- **Modern UI**: Sleek sidebar navigation with chat management

## 🛠️ Tech Stack

### Frontend
- **React** - UI framework
- **Vite** - Build tool and development server
- **UUID** - Unique thread ID generation
- **React Spinners** - Loading indicators

### Backend
- **Node.js** - Runtime environment
- **Express** - Web application framework
- **MongoDB** - Database for storing chat history
- **Mongoose** - MongoDB object modeling
- **OpenAI API** - AI chat completions
- **CORS** - Cross-origin resource sharing


## 🔧 Installation


### 1. Backend Setup

```bash
cd Backend
npm install
```

Create a `.env` file in the Backend directory:
```env
OPENAI_API_KEY=your_openai_api_key_here
MONGODB_URI=your_mongodb_connection_string_here
```

### 2. Frontend Setup

```bash
cd Frontend
npm install
```

## 🚀 Running the Application

### Start the Backend Server

```bash
cd Backend
npm start
```
The server will run on `http://localhost:8080`

### Start the Frontend Development Server

```bash
cd Frontend
npm run dev
```
The frontend will typically run on `http://localhost:5173`

## 📁 Project Structure

```
OpenGpt/
├── Backend/
│   ├── routes/
│   │   └── chat.js          # Chat API routes
│   ├── server.js            # Express server setup
│   ├── package.json         # Backend dependencies
│   └── .env                 # Environment variables (not tracked)
│
├── Frontend/
│   ├── src/
│   │   ├── App.jsx          # Main application component
│   │   ├── ChatWindow.jsx   # Chat interface component
│   │   ├── Sidebar.jsx      # Sidebar navigation component
│   │   ├── Chat.jsx         # Individual chat message component
│   │   ├── MyContext.jsx    # React Context for state management
│   │   ├── *.css            # Component styles
│   │   └── assets/          # Static assets
│   ├── public/              # Public assets
│   └── package.json         # Frontend dependencies
│
└── README.md
```

## 🔑 Key Components

### Backend
- **server.js**: Main server file with Express setup, MongoDB connection, and API routes
- **chat.js**: Handles chat requests and OpenAI API integration

### Frontend
- **App.jsx**: Main application component with context provider
- **ChatWindow.jsx**: Manages chat input/output and API calls
- **Sidebar.jsx**: Displays chat threads and navigation
- **Chat.jsx**: Renders individual chat messages
- **MyContext.jsx**: Global state management using React Context


## 🎨 Features Breakdown

1. **New Chat**: Start a fresh conversation with a new thread ID
2. **Thread Management**: Switch between different conversation threads
3. **Chat History**: View all previous messages in the current thread
4. **Loading States**: Visual feedback during API calls
5. **Responsive Design**: Works on various screen sizes


## Author

Gauri Shirke
