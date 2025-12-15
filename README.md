# Real-time Chat with Smart AI Features 💬

Modern real-time chat application with AI-powered spam detection, smart reply suggestions, content moderation, and message analytics.

## 🌟 Features

- **Real-time Messaging** - Instant messaging using WebSocket
- **AI Spam Detection** - Automatically detect and filter spam messages
- **Smart Reply Suggestions** - AI-generated quick reply options
- **Content Moderation** - AI filters inappropriate content
- **Message Analytics** - Sentiment analysis and conversation insights
- **Group Chats** - Create and manage group conversations
- **File Sharing** - Share images, documents, and media
- **Read Receipts** - See when messages are read
- **Typing Indicators** - Real-time typing status
- **Message Search** - Search through conversation history

## 🛠️ Tech Stack

**Frontend:**
- React.js
- Socket.io-client
- Material-UI
- Axios

**Backend:**
- Java Spring Boot
- Spring WebSocket
- Spring Security
- Python (AI Services)

**AI/ML:**
- Spam classification model
- Sentiment analysis
- Content moderation AI
- Smart reply generation

**Database:**
- MongoDB (Messages)
- Redis (Real-time data)

## 📋 Prerequisites

- Java 17+
- Python 3.8+
- Node.js 14+
- MongoDB
- Redis
- Maven

## 🚀 Installation

### Backend Setup

```bash
cd backend
mvn clean install
mvn spring-boot:run
```

### AI Service Setup

```bash
cd ai-service
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python app.py
```

### Frontend Setup

```bash
cd frontend
npm install
npm start
```

## 📁 Project Structure

```
realtime-chat-smart-features/
├── backend/
│   ├── src/main/java/com/chat/
│   │   ├── controller/
│   │   ├── service/
│   │   ├── model/
│   │   ├── config/
│   │   └── websocket/
│   └── pom.xml
├── ai-service/
│   ├── app.py
│   ├── spam_detector.py
│   ├── content_moderator.py
│   └── requirements.txt
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── App.js
│   └── package.json
└── README.md
```

## 🎯 Key Features

### 1. AI Spam Detection
Machine learning model trained to identify spam with 95%+ accuracy.

### 2. Smart Replies
Context-aware AI generates relevant quick reply suggestions.

### 3. Content Moderation
Automatically filters toxic language and inappropriate content.

### 4. Message Analytics
Analyzes conversation sentiment and provides insights.

## 📊 WebSocket Events

- `message:send` - Send new message
- `message:receive` - Receive message
- `typing:start` - User started typing
- `typing:stop` - User stopped typing
- `message:read` - Message read receipt
- `user:online` - User came online
- `user:offline` - User went offline

## 🔧 Configuration

`application.properties`:
```properties
spring.data.mongodb.uri=mongodb://localhost:27017/chatdb
spring.redis.host=localhost
spring.redis.port=6379
websocket.allowed-origins=http://localhost:3000
```

## 👨‍💻 Author

**Keshav Jadam**
- GitHub: [@Keshavja29](https://github.com/Keshavja29)
- LinkedIn: [Keshav Jadam](https://linkedin.com/in/keshav-jadam)
