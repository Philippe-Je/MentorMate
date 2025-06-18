# 🎓 MentorMate – AI-Powered Career Mentor Platform for Students

**MentorMate** is a personalized, AI-driven career planning web application built to help students and early job seekers map their skills to in-demand roles, analyze gaps, and recommend real-world resources and open-source projects. Think of it as an AI-powered mentor who never sleeps.

---

## 🚀 Features

| Feature                     | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| 🎯 Smart Career Quiz        | GPT-driven quiz recommends career paths (e.g., SWE, DS, Cybersecurity)     |
| 📊 Skill Gap Analyzer       | Compare resumes against desired job roles to highlight missing skills      |
| 📚 Learning Path Generator  | Custom roadmaps using curated YouTube, Coursera, or internal content       |
| 💼 Project Recommender      | Suggest GitHub repositories based on user skills and goals                 |
| 🎙️ AI Mock Interviewer      | Practice behavioral & technical interviews with GPT-powered prompts        |
| 📈 Progress Dashboard       | Visual charts for path completion, skills, certifications                  |
| 🏆 Gamification             | Earn points, badges, and milestones as you progress                        |
| 🧑‍🤝‍🧑 Collaboration         | Plan with peers, recommend resources, or co-mentor friends                |
| 🔍 Chrome Extension         | Parse job descriptions on LinkedIn to instantly get career advice         |

---

## 🧠 Why This Project Stands Out

- Combines **real-world job market data** with **personalized AI feedback**
- Targets **a real pain point** for students: _"Where do I start?"_
- Showcases a wide range of CS and product skills from backend architecture to frontend UX

---

## 🛠 Tech Stack

| Area               | Technology                                                              |
|--------------------|-------------------------------------------------------------------------|
| 🧠 AI / NLP         | OpenAI GPT-4 / Gemini API, spaCy                                        |
| ⚙️ Backend          | Python, FastAPI, REST API, Celery (for async tasks)                    |
| 🌐 Frontend         | Next.js (App Router), Tailwind CSS, Framer Motion, shadcn/ui           |
| 🗄 Database         | PostgreSQL (user data, quizzes), MongoDB (resources, resume vectors)   |
| 🔍 Scraping / APIs  | BeautifulSoup / Scrapy, LinkedIn & GitHub API                          |
| 📦 DevOps          | Docker, GitHub Actions (CI/CD), AWS/GCP, Terraform                     |
| 🔌 Chrome Extension | JavaScript + Manifest V3 + GPT API Integration                         |
| 📊 Visualization    | Chart.js, Recharts, D3.js                                               |

---

## 📐 Architecture Overview

```text
Client (React / Next.js)
    |
    | REST API Calls
    v
Backend (FastAPI)
    |
    ├── Authentication (OAuth2)
    ├── Resume Parser & Skill Analyzer (OpenAI + PDF parser)
    ├── Career Quiz Engine (LLM prompt templates)
    ├── Resource Recommender (YouTube, Coursera, GitHub APIs)
    ├── Progress Tracker Service (Postgres + Celery workers)
    |
    v
Database Layer (PostgreSQL + MongoDB)
    |
    v
External APIs (LinkedIn Jobs, GitHub, YouTube, Coursera)
```

---

## 🧪 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/mentormate.git
cd mentormate
```

### 2. Set up the Backend

```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows, use venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
```

### 3. Set up the Frontend

```bash
cd ../frontend
npm install
npm run dev
```

### 4. Configure Environment Variables

#### Backend (`backend/.env`)

```env
OPENAI_API_KEY=your_openai_key
DATABASE_URL=postgresql://user:pass@localhost/db
MONGO_URI=mongodb://localhost:27017
```

#### Frontend (`frontend/.env.local`)

```env
NEXT_PUBLIC_API_BASE_URL=http://localhost:8000
```

---

## 🌍 Live Demo

Coming soon! Potential deployment platforms:

- **Frontend**: [Vercel](https://vercel.com/) or [Netlify](https://netlify.com/)
- **Backend**: [Render](https://render.com/), [Railway](https://railway.app/), or [Google Cloud Run](https://cloud.google.com/run)

---

## 🤝 Contributing

We welcome contributions from the community!

### To contribute:

1. **Fork** the repository  
2. Create a new branch:  
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes and **commit** them  
4. Push to your fork:  
   ```bash
   git push origin feature/your-feature-name
   ```
5. Submit a **Pull Request**

> ✅ Please follow [Conventional Commits](https://www.conventionalcommits.org/) for commit messages.

---

## 📄 License

This project is licensed under the **MIT License**.  
© [Your Name]

---

## 🙌 Acknowledgments

- [OpenAI](https://openai.com/)
- [Next.js](https://nextjs.org/)
- [FastAPI](https://fastapi.tiangolo.com/)
- [Tailwind CSS](https://tailwindcss.com/)
- [GitHub REST API](https://docs.github.com/en/rest)

---

## 💬 Contact

Want to reach out or collaborate?

- 📧 phil09492@gmail.com 
