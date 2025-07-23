# 🎓 Alumni Networking Platform
## 📌 Overview
The **Alumni Networking Platform** is a **SaaS-based** web application designed to connect students with alumni for career guidance, networking, and mentorship. It includes **real-time chat**, event management, knowledge sharing, and a video call scheduling system.

## 🚀 Features
### 🔹 User Authentication
- Separate **Student** and **Alumni** logins
- Secure authentication with **JWT & Multi-Factor Authentication** (MFA)
- **Profile verification system** for alumni credentials

### 🔹 Chat System
- **Real-time messaging** using WebSockets or Firebase Firestore
- **Career-based alumni search** to find relevant alumni
- **No video calls inside chat** (for privacy)
- **File sharing capabilities** for documents and resources

### 🔹 Events & Scheduling
- Alumni can **create career guidance sessions & webinars**
- Students receive **notifications & RSVP options**
- **Scheduled Video Calls**: Students request a call, and alumni approve & schedule it
- **Calendar integration** with Google Calendar/Outlook

### 🔹 Knowledge Hub
- Alumni post **industry insights & learning resources**
- Students can **browse blogs & guides**
- **Content categorization** by industry and topics
- **Bookmark system** for saving important content

### 🔹 Alumni Recognition
- **Badging System & Leaderboard** for top contributors
- Colleges can offer **gifts & incentives** for active alumni
- **Points-based reward system** for active participation

### 🔹 AI-Powered Chatbot
- Integrated **Gemini Free API chatbot** for support & career guidance
- Appears as a **floating window** in the bottom left corner
- **Smart career recommendations** based on student profiles

## 🛠 Tech Stack
### Frontend
- **HTML, CSS, JavaScript** / **React.js**
- **Responsive Design** with Bootstrap/Tailwind CSS

### Backend
- **Node.js** with **Express.js** framework
- **WebSocket implementation** for real-time features

### Database
- **MongoDB** / **PostgreSQL**
- **Redis** for session management and caching

### Authentication
- **JWT** for secure authentication
- **Multi-Factor Authentication** (MFA)

## 🔧 Installation & Setup
### Prerequisites
- **Node.js** (v14.0 or higher)
- **MongoDB** or **PostgreSQL** database

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Suraj-Khaire-01/AlumNetwork-saas.git
```

### 2️⃣ Install Dependencies
```bash
cd backend && npm install  # Install backend dependencies
cd frontend && npm install  # Install frontend dependencies
```

### 3️⃣ Configure Environment Variables
Create a `.env` file in the root directory:
```env
# Database Configuration
MONGO_URI=your_mongodb_connection_string

# JWT Authentication
JWT_SECRET=your_jwt_secret_key

# Gemini AI API (for chatbot)
REACT_APP_GEMINI_API_KEY=your_gemini_api_key

# Cloudinary (for file uploads)
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

# Server Configuration
PORT=5000
```

### 4️⃣ Run the Application
```bash
# Start backend
node server.js

# Start frontend
npm run dev
```

## 📂 Project Structure
```
alumni-network-platform/
│
├── frontend/
│   ├── node_modules/        # Dependencies
│   ├── public/             # Static assets
│   ├── src/
│   │   ├── assets/         # Images, icons, fonts
│   │   ├── components/     # Reusable React components
│   │   ├── context/        # React context providers
│   │   ├── hooks/          # Custom React hooks
│   │   ├── pages/          # Page components
│   │   ├── utils/          # Helper functions
│   │   ├── App.jsx         # Main App component
│   │   ├── index.css       # Global styles
│   │   └── main.jsx        # Entry point
│   ├── .gitignore
│   ├── eslint.config.js
│   ├── index.html
│   ├── package-lock.json
│   ├── package.json
│   ├── postcss.config.js
│   ├── tailwind.config.js
│   └── vite.config.js
│
├── backend/
│   ├── Controllers/        # Route controllers
│   ├── Middlewares/        # Authentication & validation
│   ├── Models/            # Database models
│   ├── Routes/            # API routes
│   ├── socket/            # WebSocket configuration
│   ├── uploads/           # File uploads storage
│   ├── utils/             # Helper functions
│   ├── .env               # Environment variables
│   ├── package-lock.json
│   ├── package.json
│   └── server.js          # Main server file
│
└── README.md
```

## 🔒 Security Features
- **Input validation** and **sanitization**
- **Rate limiting** to prevent abuse
- **Data encryption** for sensitive information
- **Secure headers** implementation

## 💡 Future Enhancements
- 🔗 **LinkedIn Integration** for profile import
- 📱 **Mobile App** development with Flutter/React Native
- 🤖 **AI Resume Review System** with ML algorithms
- 🎥 **Video conferencing** integration
- 🌍 **Multi-language support**
- 📈 **Advanced analytics** dashboard

## 🤝 Contributing
📢 **Contributions are welcome!** Here's how you can contribute:

1. **Fork** the repository
2. **Create** a feature branch
3. **Commit** your changes
4. **Push** to the branch
5. **Open** a Pull Request

---
**Built with ❤️ for connecting students and alumni worldwide** 🌍
