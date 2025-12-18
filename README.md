# Manufacturing-Tracker
# Manufacturing Tracker

Manufacturing Tracker is an open-source scaffold for tracking inventory, work orders, and production. It includes a Node.js + TypeScript backend (Express + Prisma), a React + Vite frontend, and a Docker Compose setup for local development with PostgreSQL.

Quick highlights
- Backend: Node.js + TypeScript, Express, Prisma (Postgres)
- Frontend: React + Vite + TypeScript
- DB: PostgreSQL (docker-compose)
- Dockerized services and a simple CI workflow

Quickstart (Docker)
1. Copy example env:
   - cp backend/.env.example backend/.env
2. Start services:
   - docker-compose up --build
3. Seed DB:
   - docker-compose exec backend sh -c "npm run prisma:seed"

Backend API
- GET /api/health
- POST /api/auth/login (stub)
- GET /api/inventory
- GET /api/workorders

See docs/openapi.yaml for a minimal OpenAPI skeleton.

License: MIT
