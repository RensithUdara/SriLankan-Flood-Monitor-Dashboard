# Project Separation Guide

This project has been separated into two independent projects:

## 📁 Backend (`/backend`)
- FastAPI REST API
- Swagger documentation
- Data fetching services
- Database models and schemas
- Deployment configurations

**Location:** `backend/`
**Main file:** `backend/run.py`
**Docs:** `http://localhost:8000/docs`

## 📁 Frontend (`/frontend`)
- Interactive dashboard
- Real-time data visualization
- Map integration
- Responsive UI

**Location:** `frontend/`
**Main file:** `frontend/index.html`

## 🚀 Running Separately

### Backend
```bash
cd backend
pip install -r requirements.txt
python run.py
```

### Frontend
```bash
cd frontend
# Open index.html in browser or use:
python -m http.server 8080
```

## 🔗 Connecting Frontend to Backend

In `frontend/index.html`, update the API URL:
```javascript
const API_BASE_URL = 'http://localhost:8000/api';
```

## ✅ Benefits of Separation

1. **Independent Deployment** - Deploy backend and frontend separately
2. **Technology Freedom** - Upgrade or replace either part independently
3. **Team Organization** - Backend and frontend teams can work separately
4. **Scalability** - Scale frontend and backend independently
5. **Clear Responsibilities** - Cleaner project structure

## 📦 To Create Separate Repositories

1. Copy `backend/` folder to new repo: `lk-flood-api`
2. Copy `frontend/` folder to new repo: `lk-flood-dashboard`
3. Each can have its own git history and deployment pipeline
