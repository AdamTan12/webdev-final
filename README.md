# webdev-final

A pet matching app with a FastAPI backend and Supabase database.

## Backend Setup

### Prerequisites

- Python 3.11+
- A Supabase project

### Environment Variables

Create `backend/.env` with the following keys:

```
SUPABASE_URL=your_supabase_project_url
SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key
SUPABASE_JWT_SECRET=your_supabase_jwt_secret
```

These values can be found in your Supabase project under **Settings → API**.

> **Note:** A pre-filled `backend/.env` is already checked in and connected to the shared dev database — you can use it as-is without creating your own Supabase project.

### Install Dependencies

```bash
pip install -r backend/requirements.txt
```

Or with a virtual environment (recommended):

```bash
python -m venv backend/.venv
source backend/.venv/bin/activate   # Windows: backend\.venv\Scripts\activate
pip install -r backend/requirements.txt
```

### Run the Server

```bash
uvicorn app.main:app --app-dir backend --reload
```

The API will be available at `http://localhost:8000`.

Interactive docs: `http://localhost:8000/docs`

Health check: `http://localhost:8000/health`
