# SkillPulse

A unified full-stack platform for skill tracking, verification, and outcomes management.

This repository combines both the frontend and backend of the SkillPulse system into a single monorepo.

---

## 📁 Repository Structure

```
SkillPulse/
├── backend/                  # Django REST backend, database, APIs, auth & verification
│   ├── backend/              # Django core settings & WSGI/ASGI
│   ├── outcomes/             # Django app for outcomes, feedback, metrics
│   ├── SkillPulse/           # Core app configs & services
│   ├── templates/            # HTML templates
│   ├── static/ & staticfiles/# Static assets
│   ├── manage.py             # Django management script
│   └── requirements.txt      # Python dependencies
│
└── frontend/                 # Client interface (HTML5, Vanilla JS, CSS)
    ├── css/                  # Styling and themes
    ├── js/                   # Client-side API integration, auth, charts
    ├── images/               # Media and icons
    ├── index.html            # Landing / portal home
    ├── trainee-dashboard.html# Trainee portal
    ├── trainer-dashboard.html# Trainer portal
    ├── package.json          # Node scripts and configs
    └── vercel.json           # Frontend deployment configuration
```

---

## 🚀 Getting Started

### Prerequisites
- Python 3.10+
- Node.js (optional, for frontend serving / tooling)
- Git

---

### Backend Setup (Django)

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   # On Windows:
   .\venv\Scripts\activate
   # On Linux/macOS:
   source venv/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Apply database migrations:
   ```bash
   python manage.py migrate
   ```

5. Run the development server:
   ```bash
   python manage.py runserver
   ```
   The backend API will be live at `http://127.0.0.1:8000/`.

---

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Serve using any local HTTP server or live server (e.g. VS Code Live Server, or Python/Node):
   ```bash
   # Using Python
   python -m http.server 3000

   # Or using PowerShell helper script
   .\serve.ps1
   ```

3. Open your browser and navigate to `http://127.0.0.1:3000/`.

---

## 🔗 Related Repositories

- [SkillPulse-Backend](https://github.com/priyanshu-pgb/SkillPulse-Backend)
- [SkillPulse-Frontend](https://github.com/priyanshu-pgb/SkillPulse-Frontend)
