# Developer Setup Guide

## 1. Clone Repo
```
git clone https://github.com/mhaseeb-bot/inter_office_app.git
cd inter_office_app
```

## 2. Extract Project
Unzip:
```
ceo_exec_os_platform_full.zip
```

## 3. Backend Setup
```
cd backend
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
alembic upgrade head
python -m app.scripts.seed
uvicorn app.main:app --reload
```

## 4. Web Setup
```
cd web
npm install
cp .env.local.example .env.local
npm run dev
```

## 5. Mobile Setup
```
cd mobile
npm install
cp .env.example .env
npm run start
```

## 6. Key URLs
- API: http://localhost:8000
- Web: http://localhost:3000

## 7. Important Notes
- PostgreSQL recommended for production
- AI is mock by default
- RBAC seeded via script

## 8. Production
Use docker-compose.prod.yml

This guide helps any developer run the system end-to-end quickly.