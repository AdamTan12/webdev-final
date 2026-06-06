# webdev-final

A pet matchmaking app with a FastAPI backend and a vanilla JS frontend.

---

## Backend Setup

### Prerequisites

- Python 3.10+

### Environment Variables

A pre-filled `backend/.env` is already checked in and connected to the shared dev database — you can use it as-is.

If you need your own, create `backend/.env` with:

```
SUPABASE_URL=your_supabase_project_url
SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key
SUPABASE_JWT_SECRET=your_supabase_jwt_secret
```

### Install & Run

```bash
python3 -m venv backend/.venv
source backend/.venv/bin/activate
pip install -r backend/requirements.txt
cd backend && uvicorn app.main:app --reload
```

API: `http://localhost:8000` — Docs: `http://localhost:8000/docs`

> See [`backend/BACKEND.md`](backend/BACKEND.md) for full API reference.

---

## Frontend Setup

No build step or dependencies required.

Open `frontend/index.html` directly in a browser, or serve it with:

```bash
cd frontend
npx serve .
# or
python3 -m http.server
```

> See [`frontend/FRONTEND.md`](frontend/FRONTEND.md) for pages, structure, and walkthrough.
