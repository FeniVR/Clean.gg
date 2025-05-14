# Clean.gg – API Setup Guide

This guide will help you set up the backend API of Clean.gg for local development.

---

## Requirements

- Python 3.10+
- pip / venv
- PostgreSQL (or Railway DB)
- Redis (optional, for rate limiting/caching)
- Git
- (Optional) Docker

---

## 1. Clone the Repository

git clone https://github.com/your-username/clean.gg.git
cd clean.gg/clean-api


---

2. Set Up Virtual Environment

python -m venv venv
source venv/bin/activate  # on Windows: venv\Scripts\activate


---

3. Install Dependencies

pip install -r requirements.txt


---

4. Configure Environment Variables

Create a .env file in clean-api/:

DATABASE_URL=postgresql://user:password@localhost:5432/cleangg
REDIS_URL=redis://localhost:6379
SECRET_KEY=your-secret-key
DISCORD_WEBHOOK_URL=https://discord.com/api/webhooks/...

If using Railway or Supabase, paste their DB URL into DATABASE_URL.


---

5. Run Migrations (If using Alembic)

alembic upgrade head


---

6. Start the API Server

uvicorn main:app --reload

> The API will be available at http://localhost:8000




---

7. API Docs

FastAPI automatically generates Swagger UI:

http://localhost:8000/docs

http://localhost:8000/redoc



---

Optional: Docker Setup

You can also use Docker for easier setup:

docker-compose up --build

This will launch the API + PostgreSQL + Redis (if configured in docker-compose.yml)


---

Next Steps

Connect this API with the Clean.gg web panel

Integrate the Unity SDK with your game

Enable Discord webhooks and testing



---

Contact

Maintained by feni
Discord: dc.gg/killyourself


