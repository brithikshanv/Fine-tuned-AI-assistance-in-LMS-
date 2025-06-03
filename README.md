# 🎓 AI-Powered Learning Support System

An intelligent, fine-tuned AI-based academic assistant that integrates seamlessly with modern learning platforms to deliver **real-time**, **personalized**, and **context-aware** educational support to students.

## 🚀 Overview

This project implements a **fine-tuned GPT-based AI model** trained on subject-specific educational data to deliver instant academic support within a digital learning platform. The system empowers students through AI-driven tutoring, smart assessments, and adaptive learning recommendations—bridging the gaps in traditional and online education.

## ✨ Key Features

* 💬 **AI Chat Assistant** – Real-time query resolution using a fine-tuned GPT model
* 📚 **Concept Explanations** – Personalized and subject-aware answers
* 🧠 **Contextual NLP Processing** – Enhances the relevance and clarity of responses
* 📈 **Adaptive Learning Paths** – Tailors content based on user performance
* 🔐 **Role-Based Access** – Secure and customizable dashboards for students, admins, and instructors
* ⚙️ **Admin Tools** – Course/cohort creation, team management, progress tracking
* 🌍 **Multilingual Support (Prototype)** – Assistance available in Tamil and English

## 🧩 Tech Stack

| Layer      | Technology              |
| ---------- | ----------------------- |
| Frontend   | React.js                |
| Backend    | FastAPI + Uvicorn       |
| AI/ML      | OpenAI GPT (fine-tuned) |
| Database   | SQLite / MySQL          |
| Auth       | Google OAuth 2.0        |
| Deployment | GitHub, Judge0 API      |

## 🏗️ System Architecture

* **Frontend (React.js):** Responsive dashboard, real-time chat UI, task panel, and performance tracking.
* **Backend (FastAPI):** Handles authentication, session management, and communication with the fine-tuned OpenAI model.
* **AI Module:** Interprets and responds to student queries using a fine-tuned LLM trained on academic datasets.
* **Database Layer:** Manages user data, tasks, quiz records, chat history, and performance logs.

## 🖼️ Demo Screenshots

* Login with Google
* AI chat interface (including support in Tamil)
* Cohort creation and learner management
* Quiz generation and real-time feedback
* Personalized course dashboards

## 📦 Setup Instructions

```bash
# 1. Clone the repository
git clone https://github.com/your-username/ai-learning-assistant.git
cd ai-learning-assistant

# 2. Set up the environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Add environment variables
# Create a .env file with OpenAI_API_KEY, Judge0_API_KEY, DB_URL, and Google OAuth credentials

# 5. Run the application
uvicorn app.main:app --reload

# 6. Access frontend via React dev server or deployment
```

## 📂 Folder Structure

```
├── frontend/               # React.js UI
│   └── components/
├── backend/                # FastAPI backend
│   ├── api/
│   └── ai_engine/          # GPT-based query handler
├── data/                   # Training datasets
├── docs/                   # Project report, architecture diagrams
├── .env
├── requirements.txt
└── README.md
```

## 🧪 Sample Code (AI Interaction)

```python
@router.post("/chat")
async def ai_response_for_question(request: AIChatRequest):
    if request.task_type == TaskType.QUIZ:
        # Handle quiz-specific logic
    elif request.task_type == TaskType.LEARNING_MATERIAL:
        # Generate contextual feedback
    # Call OpenAI API with refined prompt
    response = openai.ChatCompletion.create(...)
    return response
```

## 🧠 Future Enhancements

* 🗣️ Voice and multilingual input
* 📊 Admin analytics dashboard
* 🎮 Gamification: badges, streaks, leaderboards
* 🤝 Collaborative whiteboards and group chat
* 📱 Mobile app with offline mode
* 🔁 Self-improving AI via feedback loops

## 📚 References

Includes citations from IEEE, ITME, SLAAI, and other educational AI conferences (listed in `docs/references.pdf`).

## 👥 Team Memebers 

Developed by final-year students of **University College of Engineering, Nagercoil**
Under the guidance of **Dr. T. Viveka**, Department of Computer Science & Engineering

* Saran S V
* Varsha Herolin A P
* Abinanth S
* Brithiksha N V

