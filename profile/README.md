# KRCraft

> Smart construction management for projects, budgets, materials, expenses and progress.

**GitHub:** https://github.com/KRCraft

## What we build

**BuildTrack** — Multi-tenant construction operations platform for projects, teams, and site delivery.

Small construction firms still run on spreadsheets, chats, and paper quotes. BuildTrack gives them a single dashboard to:

- Create and send professional quotes in minutes
- Track projects from inquiry → in-progress → completed
- Manage clients and contact history
- Plan payments / milestones
- Give clients a transparent view of progress

## Tech Stack

- **Backend:** Django 5 + Django REST Framework + SimpleJWT + PostgreSQL
- **Frontend:** Next.js App Router + TypeScript + Tailwind CSS
- **DevOps:** Docker Compose (Django:8000, Next.js:3000, PostgreSQL:5432, Redis:6379)
- **Docs/API:** Postman collection

## Repositories

- [KRCraft/BuildTrack](https://github.com/KRCraft/BuildTrack) — main monorepo (backend + frontend + docs)
- [KRCraft/.github](https://github.com/KRCraft/.github) — organization profile (this repo)

## Quickstart (BuildTrack)

```bash
# Docker (recommended)
docker compose up --build
# backend:  http://localhost:8000/api/v1/
# frontend: http://localhost:3000/
```
