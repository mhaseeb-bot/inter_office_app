# Cursor AI Guide (High-Level Understanding)

## What this project is
This is a full-stack executive operations platform:
- FastAPI backend
- Next.js web
- React Native mobile
- AI meeting intelligence

## Core flow
Meeting → Transcript → AI Summary → Action Items → Tasks

## Main modules
- Auth + RBAC
- Org (Users, Departments)
- Projects + Tasks
- Meetings + AI
- Notifications + Approvals
- KPI + Audit

## Where to look first
- backend/app/api/v1/
- web/app/
- mobile/src/

## Key patterns
- service layer in backend
- apiFetch wrapper in frontend
- token + refresh handling centralized

## How to extend
- add new module under backend/app/api/v1
- add schema + service
- expose API
- consume in web/mobile

This file is designed so AI tools like Cursor can understand architecture without reading every file.