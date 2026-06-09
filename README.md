# AI-Powered Career Assistant

A complete, production-ready web application designed to help users navigate their career. Features an advanced AI Chatbot, Mock Interview evaluator, Resume Builder, and Time Planner.

## 🎯 Overview

The Career Assistant is an intelligent platform that leverages AI to support career development through multiple tools:
- **AI Chatbot**: Get career guidance and professional advice
- **Mock Interview System**: Practice interviews with AI evaluation
- **Resume Builder**: Create ATS-optimized professional resumes
- **Time Planner**: Build personalized study and career development plans
- **Dashboard**: Track your progress and view history

## 🛠️ Tech Stack

### Frontend
- **Framework**: React.js (Vite)
- **Styling**: Tailwind CSS
- **Routing**: React Router DOM
- **HTTP Client**: Axios
- **Icons**: Lucide React

### Backend
- **Framework**: Python Flask
- **ORM**: Flask-SQLAlchemy
- **Authentication**: Flask-JWT-Extended
- **AI Integration**: Groq API (llama-3.1-8b-instant)

### Database
- **SQLite**: Development
- **PostgreSQL**: Production

## 📋 Features Included

✅ Secure user registration and login (JWT)
✅ Dashboard with progress tracking
✅ Resume Builder with ATS optimization
✅ Career AI Chatbot
✅ Mock Interview System with scoring
✅ Time Planner with study schedules
✅ Activity history and analytics

## 🚀 Quick Start

### Prerequisites
- Node.js 16+ (LTS): https://nodejs.org/
- Python 3.8+: https://www.python.org/downloads/
- Groq API Key: https://console.groq.com

### Backend Setup (Terminal 1)

```bash
cd backend
python -m venv venv
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

pip install -r requirements.txt

# Configure .env
cp .env.example .env
# Add your Groq API key to .env

python app.py
```

Backend runs on: **http://localhost:5000**

### Frontend Setup (Terminal 2)

```bash
cd frontend
npm install

# Configure .env
cp .env.example .env

npm run dev
```

Frontend runs on: **http://localhost:5173**

## 📚 Documentation

- [Setup Guide](docs/SETUP.md) - Detailed installation instructions
- [API Documentation](docs/API.md) - Complete API reference
- [Deployment Guide](docs/DEPLOYMENT.md) - Production deployment
- [Contributing Guide](docs/CONTRIBUTING.md) - How to contribute

## 🔐 Security

- Never commit `.env` files with API keys
- Use environment variables for all secrets
- Enable HTTPS in production
- Implement rate limiting
- Validate all user inputs

## 📖 Key Features Explained

### Dashboard
Track your generated resumes, study plans, and interview scores

### Resume Builder
Fill in details and generate professional markdown resumes with ATS scoring

### Career Chatbot
AI-powered conversations for career guidance and job search assistance

### Mock Interview
Generate 5 targeted questions for your role, submit answers, get AI evaluation (1-100)

### Time Planner
Create personalized study schedules based on goals and available hours

## 🐛 Troubleshooting

**Port in use?**
```bash
flask run --port 5001
npm run dev -- --port 5174
```

**CORS errors?**
- Check CORS_ORIGINS in backend .env matches frontend URL
- Clear browser cache

**Database issues?**
```bash
rm backend/career_assistant.db
python
>>> from app import db
>>> db.create_all()
>>> exit()
```

## 📄 License

MIT License - See [LICENSE](LICENSE) file

## 💬 Support

- 📧 Email: support@carierassistant.dev
- 🐛 Issues: [GitHub Issues](https://github.com/libnaansu-hash/career-assistant/issues)
- 💡 Discussions: [GitHub Discussions](https://github.com/libnaansu-hash/career-assistant/discussions)

---

**Happy Career Building! 🚀**
