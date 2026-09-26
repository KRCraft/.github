<div align="center">

<img src="https://avatars.githubusercontent.com/u/328459034?s=200&v=4" width="88" alt="KRCraft" />

# KRCraft

**Aqlli qurilish boshqaruvi — loyihalar, byudjetlar, materiallar, xarajatlar va taraqqiyot.**

*Multi-tenant construction operations platform for projects, teams, and site delivery.*

[![BuildTrack](https://img.shields.io/badge/Main-BuildTrack-2563eb?style=for-the-badge)](https://github.com/KRCraft/BuildTrack)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/KRCraft/BuildTrack)
[![Django](https://img.shields.io/badge/Django_5-092E20?style=flat-square&logo=django)](https://github.com/KRCraft/BuildTrack)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://github.com/KRCraft/BuildTrack)
[![Next.js](https://img.shields.io/badge/Next.js_15-black?style=flat-square&logo=next.js)](https://github.com/KRCraft/BuildTrack)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)](https://github.com/KRCraft/BuildTrack)
[![Docker](https://img.shields.io/badge/Docker_Compose-2496ED?style=flat-square&logo=docker&logoColor=white)](https://github.com/KRCraft/BuildTrack)

</div>

## Vision

Small construction firms still run on spreadsheets, WhatsApp, and paper quotes. **[BuildTrack](https://github.com/KRCraft/BuildTrack)** gives them a single dashboard to:

- Create and send professional **quotes** in minutes
- Track **projects** from inquiry → in-progress → completed
- Manage **clients** and contact history
- Plan **payments / milestones**
- Give clients a transparent view of progress

First usable slice: auth, company workspaces, roles, project management, dashboard, immutable audit.

## What’s inside BuildTrack

**Backend `backend/` — Django REST API :8000:**
`accounts` (JWT HttpOnly refresh) • `companies` (multi-tenant) • `projects` (DRAFT→ACTIVE→COMPLETED) • `budgets` • `expenses` • `inventory` • `workforce` • `reports` • `audit` • `dashboard`

**Frontend `frontend/` — Next.js 15 :3000:**
App Router (dashboard, projects, inventory, expenses) + Tailwind + `lib/api.ts` (Bearer + `X-Company-ID` + auto-refresh), legacy Vite SPA :5173 fallback.

**Also:** `docs/ARCHITECTURE.md` • `docs/ROADMAP.md` • `postman/` collection • `scripts/setup` + `run_dev` • `docker-compose.yml`

## Tech Stack

| Layer | Tech from BuildTrack |
| ----- | -------------------- |
| Backend | Django 5 + DRF + SimpleJWT + PostgreSQL |
| Frontend | Next.js App Router + TypeScript + Tailwind CSS |
| DevOps | Docker Compose — Django:8000, Next.js:3000, PostgreSQL:5432, Redis:6379 |
| API | Postman collection in `postman/` |

## Quickstart

```bash
# Docker (recommended)
docker compose up --build
# backend:  http://localhost:8000/api/v1/
# frontend: http://localhost:3000/
# admin:    http://localhost:8000/admin/
```

Windows: `scripts\setup.bat` then `scripts\run_dev.bat`
macOS/Linux: `./scripts/setup.sh` then `./scripts/run_dev.sh`

Env: `NEXT_PUBLIC_API_URL=http://localhost:8000/api/v1`

<div align="center">

[BuildTrack Repo →](https://github.com/KRCraft/BuildTrack) • [Architecture →](https://github.com/KRCraft/BuildTrack/blob/main/docs/ARCHITECTURE.md) • [Roadmap →](https://github.com/KRCraft/BuildTrack/blob/main/docs/ROADMAP.md)

© 2026 KRCraft • MIT (TBD)

</div>
