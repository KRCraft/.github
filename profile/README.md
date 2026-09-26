<div align="center">

<img src="https://avatars.githubusercontent.com/u/328459034?s=200&v=4" width="96" alt="KRCraft logo" />

# KRCraft

**Smart construction operations — projects, budgets, materials, expenses, and progress in one place.**

[![Org](https://img.shields.io/badge/GitHub-KRCraft-181717?style=flat-square&logo=github)](https://github.com/KRCraft)
[![BuildTrack](https://img.shields.io/badge/Featured-BuildTrack-2563eb?style=flat-square)](https://github.com/KRCraft/BuildTrack)
[![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/KRCraft/BuildTrack)
[![Django](https://img.shields.io/badge/Django-5-092E20?style=flat-square&logo=django)](https://github.com/KRCraft/BuildTrack)
[![Next.js](https://img.shields.io/badge/Next.js-15-black?style=flat-square&logo=next.js)](https://github.com/KRCraft/BuildTrack)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-4169E1?style=flat-square&logo=postgresql&logoColor=white)](https://github.com/KRCraft/BuildTrack)
[![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?style=flat-square&logo=docker&logoColor=white)](https://github.com/KRCraft/BuildTrack)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](https://github.com/KRCraft/BuildTrack)

[Explore BuildTrack →](https://github.com/KRCraft/BuildTrack) • [Organization →](https://github.com/KRCraft)

</div>

---

## About

Small construction firms still run on spreadsheets, chats, and paper quotes. **KRCraft** builds focused, production-ready tools to replace that chaos with a single operational dashboard.

Our flagship product, **[BuildTrack](https://github.com/KRCraft/BuildTrack)**, is a multi-tenant platform for:

- **Projects** — inquiry → active → completed lifecycle tracking
- **Quotes & Clients** — professional quotes in minutes, with contact history
- **Budgets & Expenses** — versions, categories, and approval flows
- **Inventory & Workforce** — materials, balances, transfers, assignments
- **Reports & Audit** — daily reports, revisions, and immutable audit records
- **Dashboard** — company-level KPIs for owners and site managers

> *Loyihalar, byudjetlar, materiallar, xarajatlar va taraqqiyot uchun aqlli qurilish boshqaruvi.*

---

## Why BuildTrack

| Problem | BuildTrack solution |
| ------- | ------------------- |
| Scattered Excel / WhatsApp / paper | Single source of truth for projects and money |
| No visibility for clients | Transparent progress and milestones |
| Manual quotes, lost history | Reusable clients, fast quotes, full history |
| Material leakage | Inventory balances + transfers + low-stock alerts |
| No accountability | Roles, audit log, expense approvals |

---

## Tech Stack

| Layer | Technology |
| ----- | ---------- |
| **Backend** | Django 5, Django REST Framework, SimpleJWT (HttpOnly refresh), PostgreSQL, Redis |
| **Frontend** | Next.js 15 App Router, TypeScript, Tailwind CSS, next-themes (dark mode) |
| **DevOps** | Docker Compose — `backend:8000`, `frontend:3000`, `db:5432`, `redis:6379`, Gunicorn + WhiteNoise |
| **API / QA** | REST `/api/v1/`, OpenAPI, Postman collection in `postman/` |
| **Auth** | JWT rotation, throttling / lockout, email verification, `X-Company-ID` multi-tenancy |

---

## Featured repository

### [KRCraft/BuildTrack](https://github.com/KRCraft/BuildTrack)
> Multi-tenant construction operations platform.

```
BuildTrack/
├── backend/    # Django REST API (accounts, companies, projects, budgets,
│               # expenses, inventory, workforce, reports, audit, dashboard)
├── frontend/   # Next.js 15 App Router + legacy Vite SPA fallback
├── docs/       # ARCHITECTURE.md, ROADMAP.md
├── postman/    # API collection
├── scripts/    # setup.bat/sh, run_dev.bat/sh
└── docker-compose.yml
```

**Quickstart:**

```bash
# Option A — Docker (recommended)
docker compose up --build
# backend:  http://localhost:8000/api/v1/
# frontend: http://localhost:3000/
# admin:    http://localhost:8000/admin/

# Option B — Windows local
scripts\setup.bat
scripts\run_dev.bat

# Option C — macOS / Linux local
chmod +x scripts/setup.sh scripts/run_dev.sh
./scripts/setup.sh
./scripts/run_dev.sh
```

Full guide: [BuildTrack README](https://github.com/KRCraft/BuildTrack#readme)

---

## Roadmap

- [x] Monorepo scaffold (Django + Next.js + Docker)
- [x] JWT auth, companies, roles, projects, dashboard, audit
- [x] Budgets, expenses, inventory, workforce, reports
- [ ] Payments / milestones, file uploads, client portal
- [ ] Email notifications, reporting, deployment (Render + Vercel)

See [`docs/ROADMAP.md`](https://github.com/KRCraft/BuildTrack/blob/main/docs/ROADMAP.md) and [`docs/ARCHITECTURE.md`](https://github.com/KRCraft/BuildTrack/blob/main/docs/ARCHITECTURE.md).

---

## Repositories

- [KRCraft/BuildTrack](https://github.com/KRCraft/BuildTrack) — main product monorepo
- [KRCraft/.github](https://github.com/KRCraft/.github) — organization profile (you are here)

---

## Contributing & Security

We welcome issues and pull requests on [`BuildTrack`](https://github.com/KRCraft/BuildTrack/issues). For security reports, please use GitHub [Security Advisories](https://github.com/KRCraft/BuildTrack/security) — do not open public issues for vulnerabilities.

---

<div align="center">

**KRCraft** — Build with clarity. Deliver on time.

© 2026 KRCraft • MIT (TBD)

</div>

